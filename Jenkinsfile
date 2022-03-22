node {
    stage('git clone') { 
       git 'https://github.com/rahulshettyacademy/DevopsBasics.git'
    }
	environment {
        NEXUS_VERSION = "nexus3"
        NEXUS_PROTOCOL = "http"
        NEXUS_URL = "yhttp://3.110.223.80:8081"
        NEXUS_REPOSITORY = "http://3.110.223.80:8081/repository/hdfc-snap"
        NEXUS_CREDENTIAL_ID = "nexus-user-credentials"
    }
    stage('maven clean') {
       sh 'mvn clean'
    }
    stage('mvn validate') {
       sh 'mvn validate' 
    }
    stage('mvn compile') {
       sh 'mvn compile'
    }
    stage('mvn test') {
       sh 'mvn test' 
    }
    stage('mvn package') {
       sh 'mvn package' 
    }
}

