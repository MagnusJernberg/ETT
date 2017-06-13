node { 
  stage ('start') {
    def userInput = input(
    id: 'userInput', message: 'Let\'s promote?', parameters: [
      [$class: 'TextParameterDefinition', defaultValue: 'build?', description: 'Environment', name: 'env']
    ])
    echo ("Build?: "+userInput)
  }

  stage('Publish build info') {
    parallel (
     "stream 1" : { 
       echo ("stream 1")
     },
     "stream 2" : {
       echo ("stream 2")
     }
    )
  }
}
