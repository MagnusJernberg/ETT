node { 
  stage ('start') {
    def userInput = input(
    id: 'userInput', message: 'Let\'s promote?', parameters: [
      [$class: 'TextParameterDefinition', defaultValue: 'Yes', description: 'Build?', name: 'Answer']
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
