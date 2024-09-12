pipeline{
    agent any
    stages{
	    stage('Build Image') {
	        steps{
	            sh 'sudo docker build -t niroshsuthagar/flaskapp'
	        }
	    }
	    stage('Deploy Container'){
		    steps{
			    sh 'sudo docker run -d -p 5000:5000 --name flaskapp niroshsuthagar/flaskapp'
		    }
	    }
    }
}
