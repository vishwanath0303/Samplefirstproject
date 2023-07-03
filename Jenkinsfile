pipeline {
	agent none  
	stages {
  	 stage('Maven Install') {
    	agent {
      	docker {
        	image 'maven:3.6.3'
        }
      }
      steps {
      	sh 'mvn clean install'
      }
    }
    stage('Docker Build') {
    	agent any
      steps {
      	sh 'docker build -t vkulkarni0303/spring-petclinic:latest .'
      }
    }
    }
  }
}