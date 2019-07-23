node{
   stage('SCM Checkout'){
     git 'https://github.com/eni-pradeep/maven-project'
   }
   stage('Compile-Package'){
      // Get Maven Home path
      def mvnHome = tool name: 'maven3.3.9', type: 'maven'
      sh "${mvnHome}/bin/mvn package"
  }
 } 
