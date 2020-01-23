node()
{

def mvnHome = tool 'M3'

stage('checkout')
{

git url="https://github.com/SnehalAj/JenkinsOnEC2MavenProject.git"

}


stage('build')
{
bat "${mvnHome}/bin/mvn -Dmaven.test.failure.ignore clean package"
   step([$class: 'JUnitResultArchiver', testResults: '**/target/surefire-reports/TEST-*.xml'])
}
}
