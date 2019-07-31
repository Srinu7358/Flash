node{

stage('SCM'){
//git clone
git 'https://github.com/Srinu7358/Flash.git'
}
stage('build the package'){
//mvn package
sh  'mvn clean package'
}
stage('archival'){
//archiving artifacts
archive 'target/*.war'
}
stage('test results'){
//test reports
junit 'target/surefire-reports/*.xml'
}
}
