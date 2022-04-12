pipeline {
   agent any

   stages {
      stage('Hello') {
         steps {
            echo 'Hello World'
         }
      }
	  stage('git repostitory') {
         steps {
            git "https://github.com/shyampandu/javasample.git"
	    sh "java -version"
         }
      }
	  stage('clean') {
         steps {
            sh "mvn clean"
         }
      }
	  stage('test') {
         steps {
            sh "mvn test"
         }
      }
	  stage('package') {
         steps {
            sh "mvn package"
         }
      }
	  stage('compile') {
         steps {
            sh "mvn compile"
         }
      }
	  
   }
}
