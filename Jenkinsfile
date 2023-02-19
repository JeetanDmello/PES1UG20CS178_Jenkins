pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c PES1UG20CS178.cpp'
                sh 'g++ -o PES1UG20CS178 PES1UG20CS178.cpp'
                echo 'build stage successfull'
            }
        }
        stage('Test'){
            steps{
                sh './PES1UG20CS'
                echo 'Test stage executed successfully'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deployed Successfully'
            }
        }
    }
    post{
        failure{
            echo 'Pipeline Failed'
        }
    }
}
