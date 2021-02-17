pipeline{
 agent { label 'master' }
 stages{
  stage('Deploy sphinx'){
   steps{
    sh """
      docker pull pardahlman/sphinx
    """
   }
  }
 }
}
