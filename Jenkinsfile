@Library("Shared") _
pipeline{
    agent {label "vinod"}
    
    stages{
        stage("Hello"){
            steps{
                script{
                    hello()
                }
            }
        }
        stage("code"){
            steps{
                script{
                    clone("https://github.com/sumitraj8930/Jenkins-Based-Project-django-notes-app.git","main")
                }
            }
            
        }
        stage("Build"){
            steps{
                script{
                    docker_build("notes-app","latest","sumitraj0157")
                }
            }
        }
        stage("Test"){
            steps{
                echo "This is testing the code"
            }
        }
        stage("Push to DockerHub"){
            steps{
                script{
                    docker_push("notes-app","latest","sumitraj0157")
                }
                
            }
        }
        
        stage("Deploy"){
            steps{
                echo "this is deploying the code"
                sh "docker-compose down || true"
                sh "docker-compose up -d"
            }
        }
    }
}
