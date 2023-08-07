pipeline {
   agent any
   stages{
      stage('Verify Branch in Linux env') {
         steps {
             sh(script:"echo ${GIT_BRANCH}")
         }
      }
      stage('Verify Branch in Windows env'){
         steps {
            pwsh(script: 'Write-Output "Hello World"')
         }
      }
   }
}