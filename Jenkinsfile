pipeline{
    agent any

    stages{
        stage("Preparation"){
            steps{
                git 'https://github.com/komalumare/Mock_Test_Que_1'
            }
        }

        stage("Clean"){
            steps{
                bat "mvn clean"
                echo "HII FROM CLEAN"
            }
        }

        stage("test"){
            steps{
                bat "mvn test"
                echo "HII FROM TEST"
            }
        }

        stage("install"){
            steps{
                bat "mvn install"
            }
        }

        stage("package"){
            steps{
                bat "mvn package"
            }
        }
    }
}
