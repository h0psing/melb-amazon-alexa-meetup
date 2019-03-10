# Step 4: Customise facts for your own skill

## Review Node JS Code
1.	Navigate back to https://aws.amazon.com and sign in
2.	Click Lambda under All Services
3.  Inspect Index.js code
![Code Index 01](https://github.com/h0psing/melb-amazon-alexa-meetup/blob/master/images/code-index-01.png)


### Intent Handler - GetNewFactHandler
Utterances (e.g. a fact, tell me a fact) that match the GetNewFactHandler will call the Node JS code within the handler below.
- <b>speechOutput</b> is the Alexa repsonse built using <b>Response Variables</b> and <b>Fact Data Array</b> below

```
const GetNewFactHandler = {
  canHandle(handlerInput) {
    const request = handlerInput.requestEnvelope.request;
    return request.type === 'LaunchRequest'
      || (request.type === 'IntentRequest'
        && request.intent.name === 'GetNewFactIntent');
  },
  handle(handlerInput) {
    const factArr = data;
    const factIndex = Math.floor(Math.random() * factArr.length);
    const randomFact = factArr[factIndex];
    const speechOutput = GET_FACT_MESSAGE + randomFact;

    return handlerInput.responseBuilder
      .speak(speechOutput)
      .withSimpleCard(SKILL_NAME, randomFact)
      .getResponse();
  },
};
```

### Response Variables
- Personalise your repsonse in your skill below

```
const SKILL_NAME = 'Space Facts';
const GET_FACT_MESSAGE = 'Here\'s your fact: ';
const HELP_MESSAGE = 'You can say tell me a space fact, or, you can say exit... What can I help you with?';
const HELP_REPROMPT = 'What can I help you with?';
const STOP_MESSAGE = 'Goodbye!';
```

### Fact Data Array
- Replace facts below with your own personalised facts

```
const data = [
  'A year on Mercury is just 88 days long.',
  'Despite being farther from the Sun, Venus experiences higher temperatures than Mercury.',
  'Venus rotates counter-clockwise, possibly because of a collision in the past with an asteroid.',
  'On Mars, the Sun appears about half the size as it does on Earth.',
  'Earth is the only planet not named after a god.',
  'Jupiter has the shortest day of all the planets.',
  'The Milky Way galaxy will collide with the Andromeda Galaxy in about 5 billion years.',
  'The Sun contains 99.86% of the mass in the Solar System.',
  'The Sun is an almost perfect sphere.',
  'A total solar eclipse can happen once every 1 to 2 years. This makes them a rare event.',
  'Saturn radiates two and a half times more energy into space than it receives from the sun.',
  'The temperature inside the Sun can reach 15 million degrees Celsius.',
  'The Moon is moving approximately 3.8 cm away from our planet every year.',
];
```

### Handler declarations
Ensure the intent handlers are added to the <b>addRequestHandlers</b> method.
```
exports.handler = skillBuilder
  .addRequestHandlers(
    GetNewFactHandler,
    HelpHandler,
    ExitHandler,
    SessionEndedRequestHandler
  )
  .addErrorHandlers(ErrorHandler)
  .lambda();
```

*Completed step-4?* Move to the [`step-5`](https://github.com/h0psing/melb-amazon-alexa-meetup/tree/Step-5-Publish-skill) to publish your skill to the Alexa sklls store.



