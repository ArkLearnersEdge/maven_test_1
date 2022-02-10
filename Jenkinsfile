node('Dev') {
    stage('ContinuousDownload_master') 
    {
     git 'https://github.com/ArkLearnersEdge/maven_test_1.git'
    }
    stage('ContinuousBuild_master') 
    {
     sh 'mvn package'
    }
  }
