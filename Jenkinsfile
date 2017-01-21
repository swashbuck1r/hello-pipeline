node {
    def mvnHome = tool 'M3'
    stage('Build') { 
      checkout scm
      sh "${mvnHome}/bin/mvn compile"
    }

    stage('Test') {
      sh "${mvnHome}/bin/mvn test"
    }
    stage('Deploy') {
      echo "Deploy it!"  
    }
}
