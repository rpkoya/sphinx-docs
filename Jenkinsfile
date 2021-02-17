pipeline{
 agent master
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
