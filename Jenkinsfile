node {
  withCredentials([
      [$class: 'UsernamePasswordMultiBinding', credentialsId: git_creds, usernameVariable: 'GIT_USER', passwordVariable: 'GIT_PASS'],
  ]){
    stage ('echo variables') {
      sh """(
        echo "User: ${GIT_USER}"
        echo "Pass: ${GIT_PASS}"
      )"""
    }
  }
}
