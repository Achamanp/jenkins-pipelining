pipeline{
    agent any
    tools{
        jdk 'jdk17'  // Correct syntax: tool_type 'tool_name'
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
