pipeline {
   agent any
   stages{
      stage('Verify Branch in Linux env') {
         steps {
             sh(script:"echo ${GIT_BRANCH}")
         }
      }
   }
}