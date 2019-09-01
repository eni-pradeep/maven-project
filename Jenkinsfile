node{
   stage('SCM Checkout'){
     git 'https://github.com/eni-pradeep/maven-project'
   }
   stage('Compile-Package'){
      // Get Maven Home path
      def mvnHome = tool name: 'Maven3.6.0', type: 'maven' //Defining Maven variable and defines Maven Home Directory
      sh "`sudo` ${mvnHome}/bin/mvn package"
  }
 } 
