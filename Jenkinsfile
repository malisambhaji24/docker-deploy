node{
  stage('SCM CHECKOUT'){
  git branch: 'main', url: 'https://github.com/malisambhaji24/docker-deploy.git'
    stage('MVN Package'){
      def mvnHome = tool name: 'maven-3', type: 'maven'
      def mvnCMD = "${mvnHome}/bin/mvn"
      sh "${mvnCMD} clean package"
    }
  }
}
