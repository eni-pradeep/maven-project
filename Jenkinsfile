node{
   stage('SCM Checkout'){
     git 'https://github.com/eni-pradeep/maven-project.git'
   }
   stage('Compile-Package'){
      // Get Maven Home path
      def mvnHome = tool name: 'Maven-3', type: 'maven' //Defining Maven variable and defines Maven Home Directory
      sh "${mvnHome}/bin/mvn package"
  }
 } 
