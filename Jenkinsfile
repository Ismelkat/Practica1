
pipeline {
  agent any
  parameters {
      //string(name: 'VERSION', defaultValue: '', description: 'version to deploy')
      choice(name: 'VERSION',choice:['1.4.8,2.07,3.0.0'], description: 'version to deploy')
      booleanParam(name: 'exectutiontest', defaultValue: '', description: '')
  }
  stages {
    stage('Initialize ') {
      steps {
        echo 'hola mundo '
      }
    }
     stage('Test ') {
       when{
          expression{
              param.exectutiontest
          }
       }
      steps {
        echo 'Aqui iria el codigo de la prueba el cual podria ser en groovy, selenio, or junit, etc  '
      }
    }
 stage('Deploy ') {
      steps {
        echo 'hola Ismelka > '
      }
    }

  }
}
