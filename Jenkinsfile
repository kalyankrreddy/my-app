node{
	stage('SCM Checkout'){
	  git 'https://github.com/kalyankrreddy/my-app'
	}
	stage('Compile-Package'){
	  // Get maven home path
	  def mvnHome = tool name: 'maven-3', type: 'maven'
	  sh "${mvnHome}/bin/mvn clean package"
	}
	stage('Email Notification'){
	mail bcc: '', body: '''Hi Welcome to Jenkins email alerts
	Thanks,
	Super''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'supermoon99999@gmail.com'
	}
	
 }
