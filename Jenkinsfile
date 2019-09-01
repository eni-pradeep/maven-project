node{
   stage('SCM Checkout'){
     git 'https://github.com/eni-pradeep/maven-project'
   }
   stage('Compile-Package'){
      // Get Maven Home path
      def mvnHome = tool name: 'Maven3.6.0', type: 'maven' //Defining Maven variable and defines Maven Home Directory
      sh "echo JAVA_HOME=$JAVA_HOME"
      sh "${mvnHome}/bin/mvn package"
  }
 } 
