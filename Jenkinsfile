#!/usr/bin/env groovy
/*
 From here: https://jenkins.io/doc/book/pipeline/
      here: https://github.com/jenkinsci/pipeline-plugin/blob/master/TUTORIAL.md
  and here: https://wilsonmar.github.io/jenkins2-pipeline/#jenkins2-highlights
*/
pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps { 
                stage '\u2776 Stage 1 - Build'
                echo "\u2600 BUILD_URL=${env.BUILD_URL}"
            }
        }
        stage('Test'){
            steps {
			    stage '\u2777 Stage 2 - Test'
                def workspace = pwd()
                echo "\u2600 workspace=${workspace}"
            }
        }
        stage('Deploy') {
            steps {
			    stage '\u2778 Stage 3 - Deploy'
				sh 'echo hello comrade'
            }
        }
    }
}
