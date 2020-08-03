pipeline {
   node any 

   stages {
      
     stages ("Build") {
       steps {
          sh "mvn -version"
          sh "mvn clean install"
       }  
     } 
   }
   
   post {
     always {
       cleanWs()
     }
   }
}
