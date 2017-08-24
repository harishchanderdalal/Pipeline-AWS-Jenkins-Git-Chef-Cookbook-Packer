node('master') {

   stage ('Spring Checkout')
   {
        dir ('spring') {
	git branch: 'dryrun', url: 'https://github.com/harishchanderdalal/pocAgility.git'
   	echo 'git clone Sucessfully'
            }
   }

   stage ('Spring Boot')
   {
	dir ('spring') {
	sh 'sudo ln -s /var/lib/jenkins/workspace/$JOB_NAME/spring/target/spring-petclinic-1.5.1.jar /etc/init.d/spring'
	sh 'sudo /etc/init.d/spring start'
        echo 'Build Spring'
            }
   }
   
   stage ('Spring UI')
   {
    	      echo 'Ip:9000'
   }

}
