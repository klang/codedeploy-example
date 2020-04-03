# codedeploy-example

** manual deployment

    tar cvf demoRevision.tar *
    aws s3 cp demoRevision.tar s3://codedeploy-402359887127
    
    
    aws codedeploy push --application-name DemoApp --s3-location s3://codedeploy-402359887127/Project1.zip --ignore-hidden-files --source -