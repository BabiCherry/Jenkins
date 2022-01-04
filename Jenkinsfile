node {
    stage('git clone') { 
       git 'https://github.com/rahulshettyacademy/DevopsBasics.git'
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

