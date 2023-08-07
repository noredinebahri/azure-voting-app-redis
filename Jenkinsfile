pipeline {
   agent any
   stages{
      stage('Verify Branch in Linux env') {
         steps {
             sh(script:"echo ${GIT_BRANCH}")
         }
      }
      stage('Docker build') {
         steps {
            sh(script: 'docker images -a')
            sh(script: """
               cd azure-vote/
               docker image -a
               docker build -t jenkins-pipeline .
               docker images -a
               cd ..
               """)
         }
      }
   }
}