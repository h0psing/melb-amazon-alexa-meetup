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
7.	Click on <b>Lambda</b> in the breadcrumb
8.	Click on <b>Applications</b> in the LH navigation menu
9.  Click on created application: serverlessrepo-alexa-meetup-workshop-nodejs-factskill
10. Scroll down to Resources and confirm the Lambda Function <b>Physical ID</b>
11. Click on <b>Functions</b> in the LH navigation menu
12.	Click on created function <b>aws-serverless-repository-alexaskillskitnodejsfact-XXXXXXXXXXXXX</b> 
![Create function 05](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/Create-function-05.png)
10.	Copy the <b>AWS Lambda ARN:</b> arn:aws:lambda:ap-southeast-2:433148507647:function:aws-serverless-repository-alexaskillskitnodejsfact-XXXXXXXXXXXXX
![Create function 06](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/Create-function-06.png)

*Completed step-2?* Move to the `step-3` branch to configure the skill to call the lambda function.



