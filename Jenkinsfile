pipeline {
    agent any

    stages {
        stage('Clone SCM') {
            steps {
                echo 'Cloning Repository'
                git 'https://github.com/wakaleo/game-of-life.git'
            }
       
            }
      stage('Build Artifact'){
          steps{
           echo 'Building war file'
           sh 'mvn clean install'
         }
       }
      }
    }
