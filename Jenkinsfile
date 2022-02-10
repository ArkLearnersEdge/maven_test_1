node('Dev') {
    stage('ContinuousDownload_loans') 
    {
     git 'https://github.com/ArkLearnersEdge/maven_test_1.git'
    }
    stage('ContinuousBuild_loans') 
    {
     sh 'mvn package'
    }   
    
}
