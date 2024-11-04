pipeline{
    agent any

    tools{
        maven "M3"
    }

    stages{
        stage("Build"){
            steps{
                sh "mv -Dmaven.test.failure.ignore=true clean pakage"
            }
        }
        stage("Test"){
            steps{
                sh "mvn test"
            }
        }
    }
}