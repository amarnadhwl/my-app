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
}
