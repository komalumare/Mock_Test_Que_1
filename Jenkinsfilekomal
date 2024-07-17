pipeline{
  agent any

  stages{
    stage("cleaning phase"){
      steps{
        bat "mvn clean"
      }
    }

    stage("testing phase"){
      steps{
        bat "mvn test"
      }
    }

    stage("packaging phase"){
      steps{
        bat "mvn package"
      }
    }

    stage("SonarQube analysis"){
      steps{
        bat "mvn sonar:sonar"
      }
    }

    stage("consolidate results"){
      steps{
        junit "**/target/surfire-reports/*.xml"
        archive "target/*.jar"
      }
    }
  }
}
