node('Dev') {
    stage('ContinuousDownload') 
    {
     git 'https://github.com/ArkLearnersEdge/maven.git'
    }
    stage('ContinuousBuild') 
    {
     sh 'mvn package'
    }   
    
}
