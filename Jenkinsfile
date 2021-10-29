node {
  stage('install') {
    sh 'yarn install;'
  }

  stage('build') {
    sh 'yarn build:dev;'
  }

  stage('upload') {
      sh 'scp -P 10086 -r dist/* root@106.14.1.16:/data/resources/rjhy/seeker-manager-center/auto-mcn/'
  }
}
