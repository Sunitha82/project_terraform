pipeline {
     agent any
	 tools {
	terraform 'Terraform'
  }
  
stages {
    stage('gitcheckout'){
	   steps {
	     git branch: 'main', url: 'https://github.com/Sunitha82/project_terraform.git'
	   }
	}
	stage('terraform initialisation'){
	   steps {
	     sh 'terraform init'
	   }
	 }
	stage('terraform showing plan'){
	   steps {
	     sh 'terraform plan'
	       
	   }
	 }
	stage('terraform apply'){
	   steps {
	     sh 'terraform apply --auto-approve'
	       
	   }
	 }
	
 }
}
