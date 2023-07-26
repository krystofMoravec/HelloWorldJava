pipeline {
  agent any

tools {  
  maven "MAVEN3"
  jdk "JDK8"
}

  stages {
    stage("Build"){
      steps {
        sh "mvn -s pom.xml -DskipTests install"
      }
    }
    stage("Test"){
      steps {
        sh "mvn -s pom.xml test"
      }
    }
  stage("Package"){
      steps {
        sh "mvn -s pom.xml package"
      }
    }

    }
  }



