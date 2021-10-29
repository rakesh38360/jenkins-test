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
        emailext body: '''Hi Welcome to jenkins email alerts
        Thanks
        Rakesh''', subject: 'Jenkins Job', to: 'rakesh38360@gmail.com'
    }
}
