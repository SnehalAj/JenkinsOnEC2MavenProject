node()
{

def mvnHome = tool 'M3'

stage('checkout')
{

git url : "https://github.com/SnehalAj/JenkinsOnEC2MavenProject.git"

}


stage('build')
{
bat "mvn clean package sonar:sonar"
}
   
     
}
