# Alexa

Requirements

- NodeJS, JS, Java
- OOP

## Understanding Custom Skills

Different Types of Skill Models

- Smart Home
  - control smart home devices, cameras, lights, locks, thermostats
  - Example: turn off living room lights
- Flash Briefing
  - provide content, News, Audio
- Video
  - Play video contents, search, TV, Movies
- List
- manage list for a user, add remove items, grocery, todo lists
- Gadget
  - receive input,echo buttons, use bluetooth, games, react to light , generate sound
- Custom
  - most flexible
    - developer defines requests the skill can handle
    - define how users invoke requests
    - define how your skill is identified
    - provide backend skill handler
    - this services incoming requests
    - define interaction model

## Custom Skill Major Components

- Interaction model
  - intents
    - specific task to be done
    - book flight, create a hotel reservation 
  - utterances
    - spoken phrase that mapped to an intent
    - "turn on the kitchen exhaust fan"
  - slots
    - user input values needed to fulfill an intent
    - departure and arrival date for book a flight
  - dialog
    - steps in a multi-turn conversation (if else)
    - to get all information from user
- Skill Handler
  - backend service, code that handles servicing your intents
  - Lambda function or self-hosted HTTPS service
  - processing financial transaction for ordering pizza
  - python, Node.js, Java
  - host in AWS/own server

## My Calculator

- operations
  - Addition, Subtraction, Multiplication, Division
    - "Alexa, ask my calculator to add 5 and 8"
    - "Alexa, aks my calculator to subtract 15 and 32"
    - "Alexa, tell my calculator to divide 54 and 8"
    - "Alexa, aks my calculator to multiply 15 and 32"

## Agenda

- design
- configuration
- code skill handler
- deploy lambda function
- test on browser/on actual device

## Deconstruction My Calculator

- Intents: Addition, Subtraction, Multiplication, Division
- Utterances: 
  - **Additon**: "Add two numbers", "Perform addition", "10 plus 35", "Add 10 and 35"
  - **Subtraction**: "Subtract two numbers", "Perform subtraction", "24 take away 35", "38 minus 15", "Subtract 29 from 56"
  - **Division**: "Divide two numbers"
"Perform division",
"24 divided by 3",
"Divide 100 by 20"
  - **Multiplication**: "Multiply two numbers"
,"Perform multiplication"
,"Multiply 24 and 4"
,"Multiply 24 by 4"
- Slots: First number, Second Number
- Invoking the Skill:
  - "Alexa, open my calculator"
  - "Alexa, tell my calculator to multiply 23 by 5"
  - "Alexa, ask my calculator to subtract 9 from 34"
  - "Alexa, ask my calculator to perform division"
