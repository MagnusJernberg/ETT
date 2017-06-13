node { 
  stage 'promotion'
  def userInput = input(
  id: 'userInput', message: 'Let\'s promote?', parameters: [
    [$class: 'TextParameterDefinition', defaultValue: 'uat', description: 'Environment', name: 'env']
  ])
  echo ("Env: "+userInput)
  parallel (
     "stream 1" : { 
       echo ("stream 1")
      },
     "stream 2" : {
       echo ("stream 1")
     }
   )
}
