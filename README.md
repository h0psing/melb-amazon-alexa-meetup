# Step 1: Create Alexa Skill

As a first step, we're going to create an Alexa Skill and introduce you to key components: 
Innovation name
Intents
Utteranes

We're going to need to configure both our Alexa skill and AWS, which will require a bit of back and forth between the two services. Let's start on AWS' side as we'll need to get our server running before we can configure our Alexa skill.

## Create Alexa Skill
1.	Navigate to https://developer.amazon.com/alexa and sign in
2.	Hover over <b>Your Alexa Consoles</b> and select Skills
3.	Click Create Skill
4.	Enter Skill name: Workshop Fact Skill, Default language: English (AU), Skill model: Custom
5.	Click Create skill
6.	Select: Start from scratch and click Choose
7.	Click Invocation
a.	Should be common words
b.	Should be dictionary words
c.	Acronyms and product names are risky
d.	Check out the rules on the page
8.	Click Intents
9.	Click Add Intent 
10.	Create custom intent: GetNewFactIntent
a.	Remember capitals 
11.	Click Create custom intent
12.	Add sample utterances
a.	Recommend 5-10-20 to capture of different ways to understand
b.	A fact, a space fact, tell me a fact, tell me trivia, give me trivia, give me some information, give me something
c.	Please generally doesn’t change the meaning of the request 
d.	Fuzzy match – I want a fact should match even though it’s not explicitly stated
13.	Click Save Model
14.	Click Build Model
15.	Click Endpoint
16.	Select AWS Lambda ARN
17.	Default Region: arn:aws:lambda:us-east-1:1234567890:function:workshop-getting-started-alexa-skill
18.	Click Save Endpoints
19.	Click Test
20.	Skill testing is enabled in: Development
a.	Also can test directly on Amazon Echo device logged in as the same email
21.	Open workshop fact skill
22.	Check JSON input and output


