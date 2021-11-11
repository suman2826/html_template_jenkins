pipeline {

  agent "any"

  environment {
    MAIL= "sumangoel151@gmail.com"
  }

  stages{
    stage("Init pipeline"){
      soteps{
        script{
          echo "Hello everyone"
      }
    }
    }
    stage("Sending mail"){
      steps{
        script{
          emailext mimeType: 'text/html',
                  body: '${SCRIPT,template="template.html"}', 
                  subject: 'Selenium: Job ' 
                  to: "${MAIL}"
        }
      }
    }

    }
}
