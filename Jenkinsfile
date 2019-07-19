#!groovy
node(){
    def mvnHome = tool name: 'maven3.6.1', type: 'maven'
    stage('checkout'){
     git branch: 'development', credentialsId: '47b377ac-ab96-42af-9e49-bf6720b60d7f', url: 'https://github.com/selva-institute/java-web-app-docker.git'
    //    git branch: 'development', credentialsId: '47b377ac-ab96-42af-9e49-bf6720b60d7f', url: 'https://github.cker.git'
    }
    stage('BuildArtifact'){
      sh "${mvnHome}/bin/mvn clean package"  
    }
}
