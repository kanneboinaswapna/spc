pipeline {
    agent { label 'first'}
    tools { jdk 'jdk-17'}
    stages {
        stage ('vcs') {
            steps{
               git branch: 'main', url:"https://github.com/kanneboinaswapna/spring-petclinic.git"
            }         
        }
        stage ('build') {
       steps {
         sh "mvn install"
       }
    }
    } 
}
