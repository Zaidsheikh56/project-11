pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                git 'https://github.com/Pritam-Khergade/student-ui.git' 
            }
        }
         stage('Hello11') {
            steps {
                sh'''
                sudo yum update && sudo yum install maven -y
                mvn clean install
                '''
            }
        }
    }
}
