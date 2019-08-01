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
     
   
		
sh 'cp C:\\Users\\GATEWAY\\.jenkins\\workspace\\DroovyDeployement\\target\\JenkinsWar.war C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps\\'
}

}
