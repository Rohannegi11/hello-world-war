pipeline{
    agent any
    tools{
        maven '3.8.1'
    }
    stages{
        stage('generate war file'){
            steps{
                sh 'mvn clean package'
            }
            post{
                success{
                    echo 'Archiving the Artifacts'
                    archiveArtifacts artifacts: '**/*.war'
                }
            }
             
        }
        stage('deploy to tomcat server'){
            steps{
               deploy adapters: [tomcat9(credentialsId: '1f1232ff-c9cc-4587-a962-4c3130541b78', path: '', url: 'http://13.48.45.146:8080/')], contextPath: null, war: '**/*.war'
            }
        }
    }
}
