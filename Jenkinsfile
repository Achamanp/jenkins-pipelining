pipeline{
    agent any
    stages{
        stage("compile"){
            steps{
                sh 'javac Test.java'
            }
        }
        stage("run"){
            steps{
                sh 'java Test'
            }
        }
    }
    post{
        always{
            echo 'Always'  // Use echo step directly
        }
        success{
            echo 'Success'
        }
        failure{
            echo 'Failure'
        }
    }
}
