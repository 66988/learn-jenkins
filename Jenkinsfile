def function1()
{
  print "This is a function class"
}
def function2()
{
  print " If Condition not successful"
}
node('workstation'){
  def x = 10
  env.y = 20

  stage('Variable'){
    print x
    sh 'echo y - ${y}'
  }

  stage('Function calling'){
       function1()
    }
  if(x>20)
  {
  stage('if condition')
  {
    function1()
  }
  }
  else
  {
    stage('else condition')
      {
        function2()
      }
  }

}