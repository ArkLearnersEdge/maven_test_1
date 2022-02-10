node('Dev') {
    stage('ContinuousDownload_Loans') 
    {
     git 'https://github.com/ArkLearnersEdge/maven_test_1.git'
    }
    stage('ContinuousBuild_ Loans') 
    {
     sh 'mvn package'
    }
    stage('ContinuousDeployment_ Loans')
    {
        sh 'scp /home/ubuntu/.jenkins/workspace/master/webapp/target/webapp.war ubuntu@172.31.10.108:/var/lib/tomcat8/webapps/testapp.war'
    }
    stage('ContinuousTesting_ Loans') 
    {
     git 'https://github.com/ArkLearnersEdge/FunctionalTesting.git'
     sh 'java -jar /home/ubuntu/.jenkins/workspace/master@2/testing.jar'
    }
    stage('ContinuousDelivery_ Loans')
    {
        sh 'scp /home/ubuntu/.jenkins/workspace/master/webapp/target/webapp.war ubuntu@172.31.23.247:/var/lib/tomcat8/webapps/Prodapp.war'
    }   	
}
