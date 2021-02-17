pipeline{
 agent { label 'master' }
 stages{
  stage('Deploy sphinx'){
   steps{
    sh """
      pwd
      docker run -d --name sphinx-docker -v "{pwd}":/docs -p 80:8000 pardahlman/sphinx
      docker exec sphinx-quickstart -q -p demo -a ravi
      ls -lrt
    """
   }
  }
 }
}
