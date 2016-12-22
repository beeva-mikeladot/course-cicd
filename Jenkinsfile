node('master') {
  stage('Checkout') {
    deleteDir()
    git credentialsId: '55c4080a-7c9d-4c72-9e04-e218ab80bd4e', url: 'git@github.com:beeva-mikeladot/course-cicd.git'
  }
  stage('Test') {
    sh './simplehttpserver/tests/nittests.sh ./simplehttpserver/'
  }
}
