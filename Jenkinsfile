pipeline {

	agent {

			label 'built-in'

			}

	stages {
			
			stage ('install apache'){
			steps {
			sh "yum install httpd -y"
					} 
			
			}
			
			stage ('start apache') {
			
			steps {
			sh "service httpd start"
			
				}
			}
			
			
			stage ('deploy index.html'){
			steps {
			sh " cp -r index.html /var/www/html/"
			
			}
			
			}
	}

}
