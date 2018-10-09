node{
  stage('SCM checkout')
  {
  git 'https://github.com/amarnadhwl/my-app'
  }
  stage('compile package')
  {
  sh 'mvn package'
  }
}
