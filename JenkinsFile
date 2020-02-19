pipeline {
   agent any

   stages {
      stage('init') {
         steps {
            echo 'Hello World'
            echo 'Foo Bar'
         }
      }
      stage('plan') {
         steps {
            echo 'Hello World'
         }
      }
    stage('approval') {
      options {
        timeout(time: 1, unit: 'MINUTES') 
      }
      steps {
        input 'approve the plan to proceed and apply'
      }
    }
      stage('apply') {
         steps {
            echo 'Goodbye'
         }
      }
   }
}
