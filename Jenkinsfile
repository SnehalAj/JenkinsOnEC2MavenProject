node()
{

def mvnHome = tool 'M3'

stage('checkout')
{

git url : "https://github.com/SnehalAj/JenkinsOnEC2MavenProject.git"

}


stage('build')
{
bat "${mvnHome}/bin/mvn clean test sonar:sonar"
}
   
     
}
