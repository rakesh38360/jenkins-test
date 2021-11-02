node{
    stage('SCM Checkout'){
         git 'https://github.com/javahometech/my-app'
    }
    stage('Compile-Package'){
	    //Get maven home path
	    def mvnHome = tool name: 'maven', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
    }
    stage('Email Notification'){
        emailext body: '''Hi,
        This is a Jenkins test email.

        Thanks,
        Rakesh Carpenter''', subject: 'test', to: 'rakesh.carpenter@hotmail.com'
    }
}
