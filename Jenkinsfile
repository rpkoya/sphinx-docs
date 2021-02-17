pipeline{
 agent { label 'master' }
 stages{
  stage('Deploy sphinx'){
   steps{
    sh """
      pwd
      docker run -d --rm --name sphinx-docker -v /tmp/demo-docs:/docs -p 80:8000 pardahlman/sphinx
      docker exec sphinx-docker sphinx-quickstart -q -p demo -a ravi
      ls -lrt /tmp/demo-docs
    """
   }
  }
 }
}
