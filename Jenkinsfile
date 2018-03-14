#! groovy
node{
 stage('Source'){
     git 'https://github.com/RamDevopsapp/Ant-WebProject-1.git'
 }
 
 stage('Build'){
    
    bat "ant -f build-mt.xml" 
 }
 stage('Send Email'){
     mail bcc: 'kalupukuriram512@gmail.com', body: 'Buils is done', cc: '', from: '', replyTo: '', subject: 'Build Status', to: 'devopstrainingblr@gmail.com'
 }
 /*stage('Archive'){
  archiveArtifacts '/Users/bhaskarreddyl/.jenkins/workspace/Pipeline-Project-Ant-Web/dist/SampleAntProject.war'
 }*/
}
