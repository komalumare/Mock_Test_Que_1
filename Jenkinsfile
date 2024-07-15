Pipeline{
    agent any

    stages{
        stage("Preparation"){
            git 'https://github.com/komalumare/Mock_Test_Que_1.git'
        }

        stage("Clean"){
            bat "mvn clean"
        }

        stage("test"){
            bat "mvn test"
        }

        stage("install"){
            bat "mvn install"
        }

        stage("package"){
            bat "mvn package"
        }
    }
    
}
