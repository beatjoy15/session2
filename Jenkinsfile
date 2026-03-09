pipeline{
agent any
  stages
  {
    stage('Checkout'){
    steps{

      git 'https://github.com/beatjoy15/session2.git'
    }
  }
stage('Publish')
  {
    steps{
    publishHTM([
      allowmissing:true,
      alwaysLinktoLastBuild:false,
      KeepAll:false,
      reportDir:'.',
      reportFiles:'Hello.html',
      reportName:'Pipeline HTML'
      ])
  }
  }
} 
}
