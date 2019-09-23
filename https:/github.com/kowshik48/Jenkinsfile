pipeline{
	       agent{
		          node{
			label 'master'
		}
	}
	stages{
		stage('ansiable started'){
			steps{
				sh 'echo "Started...!" '
			}
		}
stage('terraform start'){
			steps{
				sh 'cd /home/ubuntu/ansible; sudo ansible-playbook -i ec2.py -u devops apache-tomcat.yml'
			}
		}
stage('ansiable ended'){
			steps{
				sh 'echo "Ended......!" '
			}
}
    
  }
}
