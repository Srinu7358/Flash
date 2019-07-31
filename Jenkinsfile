node{

stage('SCM'){
//git clone
git 'https://github.com/Srinu7358/Flash.git'
}
stage('build the package'){
//mvn package
sh  'mvn clean package'
}
  stage('Deploy') {
     
       steps {
       
         echo 'Deploying'
	
			script{
		
sh "copy /var/lib/jenkins/workspace/GroovyDeployement/target/JenkinsWar.war" "/var/lib/tomcat8/webapps"
}
}
}

}
