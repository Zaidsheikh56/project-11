pipeline {
  agent {
    label "slave"
  }
   stages {
     stage('git install') {
        steps {
             sh'''
             sudo yum update -y
             sudo yum install git -y
             '''
        }
     }
     stage('git checkout') {
       steps {
          git 'https://github.com/Pritam-Khergade/student-ui.git'
       }
     }
     stage('build-stage') {
        steps {
             sh'''
             sudo yum install maven -y 
             mvn clean install
             '''
        }

     }
   }
}
          
