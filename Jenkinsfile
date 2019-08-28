 pipeline{
stages{
stage('SCM'){
//git clone
git 'https://github.com/Srinu7358/Flash.git'
}
stage('build the package'){
//mvn package
sh  'mvn clean package'
}
  stage('Deploy') {
     
   
		
//sh 'cp C:\\Users\\GATEWAY\\.jenkins\\workspace\\DroovyDeployement\\target\\JenkinsWar.war C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps\\'


}
post {
    failure {
      // notify users when the Pipeline fails
      mail to: 'srinuvasarao7358@gmail.com',
          subject: "Failed Pipeline: ${currentBuild.fullDisplayName}",
          body: "Something is wrong with ${env.BUILD_URL}"
    }
	}
}
}
   
