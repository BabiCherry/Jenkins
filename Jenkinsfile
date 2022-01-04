node {    
    stage('Git clone') {
       git 'https://github.com/rahulshettyacademy/DevopsBasics.git'
    }
    stage('maven clean') {
       sh 'mvn clean'
    }
    stage('maven validate') {
       sh 'mvn validate'
    }
    stage('maven compile') {
       sh 'mvn compile'
    }
    stage('maven test') {
       sh 'mvn test'
    }
    stage('maven package') {
       sh 'mvn package'
    }
}

