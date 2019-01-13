# Step 1: Create Alexa Skill

As a first step, we're going to create an Alexa Skill and introduce you to the following key components: 
- Invocation name
- Intents
- Utteranes

We're going to need to configure both our Alexa skill and AWS, which will require a bit of back and forth between the two services. Let's start with creating a new Alexa skill.

## Create Alexa Skill
1.	Navigate to https://developer.amazon.com/alexa and sign in
2.	Hover over <b>Your Alexa Consoles</b> and select <b>Skills</b><br /><br />
![Open skills console](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/open-skills-console.png)
<br />
3.	Click <b>Create Skill</b> <br />
4.	Enter <b>Skill name:</b> Workshop Fact Skill 
<br />     <b>Default language:</b> English (AU)
<br />     <b>Skill model:</b> Custom <br /><br />

![Create skill 01](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/Create-skill-01.png)

5.	Click <b>Create skill</b>
6.	Select: <b>Start from scratch</b> and click <b>Choose</b> <br />
![Create skill 02](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/Create-skill-02.png)
7.	Click <b>Invocation</b> and enter value for <b>Skill Inovcation Name</b>
<br />    a.	Should be common words
<br />    b.	Should be dictionary words
<br />    c.	Acronyms and product names are risky
<br />    d.	Check out the rules on the page
8.	Click <b>Intents</b>
9.	Click <b>Add Intent</b>
![Add intent 01](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/Add-intent-01.png)
10.	Enter custom intent name: <b>GetNewFactIntent</b>
<br />  a.	Remember capitals 
<br />  a.	Make it meaningful 
![Add intent 02](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/Add-intent-02.png)
11.	Click <b>Create custom intent</b>
12.	Add sample <b>utterances</b>
<br />  a.	Recommended to have 15-20 to capture of different ways users can request the same intent
<br />  b.	E.g. a fact, a space fact, tell me a fact, tell me trivia, give me trivia, give me some information, give me something, please tell me a fact
<br />  c.	<b>Please</b> generally doesn’t change the meaning of the request 
<br />  d.	Fuzzy match – <i><b>I want a fact</b></i> should match even though it’s not explicitly stated <br />
![Add intent 03](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/Add-intent-03.png)
13.	Click <b>Save Model</b>
14.	Click <b>Build Model</b>
15.	Click <b>Endpoint</b>
16.	Note the  AWS Lambda ARN <br />
![Note ARN Endpoint 01](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/arn-endpoint-01.png)

*Completed step-1?* Move to the `step-2` branch to create your lambda function and we will come back to the endpoint to finalise.



17.	Default Region: arn:aws:lambda:us-east-1:1234567890:function:workshop-getting-started-alexa-skill




18.	Click <b>Save Endpoints</b>
19.	Click <b>Test</b>
20.	Skill testing is enabled in: Development
<br />  a.	Also can test directly on Amazon Echo device logged in as the same email
21.	Open workshop fact skill
22.	Check JSON input and output


