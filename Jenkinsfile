pipeline{
 agent any
 environment{
     PATH= "/opt/maven/bin:$PATH"
 }
 stages{
     stage('git clone'){
         steps{
             git url: 'https://github.com/Tharun7152/sparkjava-war-example.git', branch: 'master'
         }
     }
     stage("build"){
         steps{
             sh 'mvn clean install'
         }
     }
 }
 
}
