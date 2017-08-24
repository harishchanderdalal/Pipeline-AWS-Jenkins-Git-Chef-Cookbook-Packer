node('master') {

   stage ('Spring Checkout')
   {
        dir ('spring') {
        git 'https://github.com/harishchanderdalal/spring-petclinic.git'
   	      echo 'git clone Sucessfully'
            }
   }

   stage ('Spring Boot')
   {
         dir ('spring') {
            echo 'Build Spring'
            }
   }
   
   stage ('Spring UI')
   {
    	      echo 'Ip:9000'
   }

}
