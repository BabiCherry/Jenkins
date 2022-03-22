node {
    stage('git clone') { 
       git 'https://github.com/rahulshettyacademy/DevopsBasics.git'
    }
    stage('upload war file to nexus'){
       'nexusArtifactUploader credentialsId: 'nexus-user-credentials', groupId: 'com.example.maven-project', nexusUrl: '3.110.223.80:8081', nexusVersion: 'nexus3', protocol: 'http', repository: 'http://3.110.223.80:8081/#browse/browse:hdfc-snap', version: '1.0-SNAPSHOT'
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

