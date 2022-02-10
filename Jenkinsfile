node('Dev') {
    stage('ContinuousDownload_PB') 
    {
     git 'https://github.com/ArkLearnersEdge/maven_test_1.git'
    }
    stage('ContinuousBuild_PB') 
    {
     sh 'mvn package'
    }
  }
