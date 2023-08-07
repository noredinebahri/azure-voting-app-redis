pipeline {
   agent any
   stages{
      stage('Verify Branch in my perso') {
         steps {
             sh(script:"echo ${GIT_BRANCH}")
         }
      }
      stage('get all information about env git'){
         steps {
            echo "git env: ${env}"
         }
      }
   }
}