node('master') {

   stage ('Spring Checkout')
   {
        git 'https://github.com/harishchanderdalal/spring.git'
   		   echo 'git clone Sucessfully'
   }

   stage ('Build Spring')
   {
        sh 'nohup ./mvnw clean install  </dev/null >/dev/null 2>&1 &'
   		echo 'Spring Build Sucessfull'
   }

   stage ('Spring UI')
   {
    	echo 'Ip:8080'
   }

   stage ('Vagrant Checkout')
   {
       git 'https://github.com/harishchanderdalal/vagrantEc2Tomcat.git'
   		echo 'Vagrant Clone'
   }

   stage ('Vagrant Build')
   {
      sh 'export key=${key}'
      sh 'export access=${access}'
      sh 'export keypair=${keypair}'
      sh 'export region=${region}'
      sh 'export sgroup=${sgroup}'
      sh 'export tag=${tag}'
      sh 'export owner=${owner}'                    
      sh './vagrantfile.sh > Vagrantfile'
         echo 'Vagrantfile Created'
   }

   stage ('vagrant box')
   {
      sh 'vagrant box add dummy https://github.com/mitchellh/vagrant-aws/raw/master/dummy.box'
      echo 'Vagrant Ready'
   }

   stage ('Ec2 Provison')
   {
      sh 'vagrant up --provider=aws'
          echo 'Ec2 Created'
   }
}
