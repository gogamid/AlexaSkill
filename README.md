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
