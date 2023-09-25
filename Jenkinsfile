pipeline { 
 agent {
   node {
     label 'maven-agent'
     }
   }
environment { 
  PATH = "/opt/apache-maven-3.0.1/bin:$PATH" //path of mvn command $PATH- existing path
 }
 stages {
   stage ('build') { 
     steps { 
             sh 'mvn clean deploy'
            }
      }
  }
}
