node('master') {

   stage ('Spring Checkout')
   {
        dir ('spring') {
	git 'https://github.com/harishchanderdalal/pocAgility.git'
   	echo 'git clone Sucessfully'
            }
   }

   stage ('Spring Boot')
   {
	dir ('spring') {
	sh 'sudo /etc/init.d/spring start'
        echo 'Build Spring'
            }
   }
   
   stage ('Spring UI')
   {
    	      echo 'Ip:9000'
   }

}
