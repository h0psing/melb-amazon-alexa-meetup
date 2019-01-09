# Step 1: Create Alexa Skill

As a first step, we're going to create an Alexa Skill and introduce you to key components: 
Innovation name
Intents
Utteranes

We're going to need to configure both our Alexa skill and AWS, which will require a bit of back and forth between the two services. Let's start on AWS' side as we'll need to get our server running before we can configure our Alexa skill.

## Create Alexa Skill
1.	Navigate to https://developer.amazon.com/alexa and sign in
2.	Hover over <b>Your Alexa Consoles</b> and select <b>Skills</b>
3.	Click <b>Create Skill</b>
4.	Enter <b>Skill name:</b> Workshop Fact Skill Default language: English (AU), Skill model: Custom
5.	Click Create skill
6.	Select: Start from scratch and click <b>Choose</b>
7.	Click <b>Invocation</b> and enter value for <b>Skill Inovcation Name</b>
    a.	Should be common words
    b.	Should be dictionary words
    c.	Acronyms and product names are risky
    d.	Check out the rules on the page
8.	Click <b>Intents</b>
9.	Click <b>Add Intent</b>
10.	Create custom intent: GetNewFactIntent
a.	Remember capitals 
11.	Click <b>Create custom intent</b>
12.	Add sample utterances
a.	Recommend 5-10-20 to capture of different ways to understand
b.	A fact, a space fact, tell me a fact, tell me trivia, give me trivia, give me some information, give me something
c.	Please generally doesn’t change the meaning of the request 
d.	Fuzzy match – I want a fact should match even though it’s not explicitly stated
13.	Click <b>Save Model</b>
14.	Click <b>Build Model</b>
15.	Click <b>Endpoint</b>
16.	Select AWS Lambda ARN
17.	Default Region: arn:aws:lambda:us-east-1:1234567890:function:workshop-getting-started-alexa-skill
18.	Click <b>Save Endpoints</b>
19.	Click <b>Test</b>
20.	Skill testing is enabled in: Development
a.	Also can test directly on Amazon Echo device logged in as the same email
21.	Open workshop fact skill
22.	Check JSON input and output


