# Step 2: Create Lambda Function


# Create Lambda Function
1.	Navigate to https://aws.amazon.com and sign in
2.	Click <b>Lambda</b> under <b>All Services</b>
3.	Click <b>Create function</b>
![Create function 01](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/Create-function-01.png)
4.	Select <b>AWS Serverless Application Repository</b> and click 
<b>alexa-skills-ski-nodejs-factskill</b> <br />
![Create function 02](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/Create-function-02.png)
5.	Under <b>Application settings:</b> enter <b>Application name:</b> alexa-meetup-workshop-nodejs-factskill
![Create function 03](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/Create-function-03.png)
6.	Click <b>Deploy</b>
<br />  a.	Wait for resources to show <b>CREATE_COMPLETE</b> 
![Create function 04](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/Create-function-04.png)
7.	Go back to Applications and open application
8.	Note the arn:aws:lambda:us-east-1:1234567890:function:workshop-getting-started-alexa-skill

![Create function 05](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/Create-function-05.png)
![Create function 06](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/Create-function-06.png)



Go to IAM

10. Go back to Alexa Dev
Click Endpoint (LHS)

Slect AWS Lambda ARN

Pastearn:aws:lambda:ap-southeast-2:433148507647:function:aws-serverless-repository-alexaskillskitnodejsfact-134BMR79UZ1UQ
into Default Region:
![Configure skill endpoint 06](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/Configure-skill-endpoint-01.png)
Click Save Endpoints

