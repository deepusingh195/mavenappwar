node{
stage('SCM Checkout'){
git 'https://github.com/deepusingh195/mavenappwar'
}
stage('Compile-Package'){
sh'mvn package'
}
  stage('Deploy to Tomcat'){
    sh 'scp -o StrictHostKeyChecking=no target/*.war root@localhost:/soft/apache-tomcat-7.0.92/webapps/'
  }
}

