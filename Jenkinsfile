
node {
  withCredentials([
      [$class: 'UsernamePasswordMultiBinding', credentialsId: "1234567", usernameVariable: 'dockeruser', passwordVariable: 'dockerpass'],
  ]){
    stage ('echo variables') {
      sh """(
       Docker login -u $dockeruser -p $dockerpass
      )"""
    }
  }
}
