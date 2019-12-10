node{
stage('SCM Checkout'){
git 'https://github.com/deepusingh195/mavenappwar'
}
stage('Compile-Package'){
sh'mvn package'
}
  stage('Deploy to Tomcat'){
    sh 'cp -r -o StrictHostKeyChecking=no target/*.war /soft/apache-tomcat-7.0.92/webapps/'
  }
}

