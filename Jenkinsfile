pipeline {
  agent any
  stages {
    stage('Plan') {
      steps {
        echo 'We will first create plan that how many sprinti are requried'
      }
    }

    stage('Code') {
      steps {
        echo 'Developer will create code'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Sonar team will test the code'
          }
        }

        stage('Build') {
          steps {
            echo 'Jenkisn will convert code into one Artifact'
          }
        }

        stage('Release') {
          steps {
            echo 'After that Team will Rease code after test'
          }
        }

        stage('Deploy') {
          steps {
            echo 'Will deploy code in Applicatin server'
          }
        }

        stage('Operate') {
          steps {
            echo 'We can operate & access through internet'
          }
        }

      }
    }

  }
}