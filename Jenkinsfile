pipeline{
    agent any;
    
    parameters {
        string(name: 'IMAGE_VERSION', defaultValue: 'latest', description: 'Image tag')
    }
    stages{
        stage("Code Clone"){
            steps{
                git url: "https://github.com/himanshi1107/BankApp_DevSecOps_EKS.git", branch: "main"
            }
        }
        stage("Trivy Scan"){
            steps{
                sh "trivy fs ."
            }
        }
        stage("Build"){
            steps{
                sh "docker build -t bankapp-eks:${params.IMAGE_VERSION} ."
            }
        }
        stage("Push"){
            steps{
               withCredentials([usernamePassword(
                credentialsId: "dockerHub",
                usernameVariable: "dockerHubUser",
                passwordVariable: "dockerHubPass")]) {
                    sh '''
                        docker login -u $dockerHubUser -p $dockerHubPass
                        docker image tag bankapp-eks:${IMAGE_VERSION} $dockerHubUser/bankapp-eks:${IMAGE_VERSION}
                        docker push $dockerHubUser/bankapp-eks:${IMAGE_VERSION}
                    '''
                }

            }
        }
    }
}
