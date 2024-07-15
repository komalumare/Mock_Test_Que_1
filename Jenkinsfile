Pipeline{
    agent any

    stages{
        stage("Preparation"){
            git 'https://github.com/jglick/simple-maven-project-with-tests.git'
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
