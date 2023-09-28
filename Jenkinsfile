node('workstation'){
  def x = 10
  env.y = 20
  stage('Variable'){
    print x
    sh 'echo y - ${y}'
  }
}