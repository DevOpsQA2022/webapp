pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'build succesfully'
            }
        }
      stages {
        stage('Deloy') {
            steps {
                deploy adapters: [tomcat8(credentialsId: 'a113e3b9-6ba1-471a-8989-c99776136ead', path: '', url: 'http://localhost:9090/')], contextPath: null, war: '**/*.war'
                echo 'successfully'
            }
        }
      
    }
}
