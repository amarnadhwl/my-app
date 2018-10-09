node{
  stage('SCM checkout')
  {
  git 'https://github.com/amarnadhwl/my-app'
  }
  stage('compile package')
  {
    def mvnhome= tool name: 'mvn-3', type: 'maven'
    sh "${mvnhome}/bin/mvn package"
  }
  stage('Email notification')
  {
    mail bcc: '', body: 'Test from jenkins', cc: '', 
      from: '', replyTo: '',
      subject: 'Test from Jenkins', 
      to: 'munagawl@gmail.com'
  }

}
