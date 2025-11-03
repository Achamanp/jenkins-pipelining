pipeline{
    agent any
    tools{
        jdk 'jdk17'
    }
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
            echo 'Always'
        }
        success{
            echo 'Success'
        }
        failure{
            echo 'Failure'
        }
    }
}
