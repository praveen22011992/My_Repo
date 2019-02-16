node ('master') {
    stage('Code Check out') {
                git branch: 'master',
                credentialsId: '1c94903a-36c5-4919-a5fc-271fa4f76459' ,
                url: 
                  
  }
    stage('Update or Create Stack') {
     // first cloud formatation stack
        try {sh 'aws cloudformation update-stack --stack-name wpo-devops-praveen-demo --template-body file://ec2.yml' } catch (Exception e) {}
        try {sh 'aws cloudformation create-stack --stack-name wpo-devops-praveen-demo --template-body file://ec2.yml' } catch (Exception e) {}
                                               
    }
}
