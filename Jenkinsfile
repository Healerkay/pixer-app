pipeline{
    agent any
    stages{
        stage("Test"){
            steps{
                sh '''
                       echo "Hello World"
                   '''
            }
        }
        stage("Build now"){
            steps{
                sh '''
                      ## Get the project
                       

                       sudo docker build -t healerkay/pixer:latest .

                       sudo docker run -d -p 801:80 healerkay/pixer:latest

                   
                   
                   
                   '''
            }
        }
    }
}