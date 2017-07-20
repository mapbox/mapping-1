# Mapping the Resistance 

## **Overview** 

Resistbot users are sending ~300K messages/day and many users have requested transparency around local statistics related to usage. 

Questions users have : 

- How many people have sent emails/faxes in my [state, county]? 
- What’s the bounce rate for my reps? 
- What is the general sentiment of my fellow constituents when they contact their reps? 

By creating a map that highlights user data, individuals will be able to see political activity based geographic location(s). 

The Resistbot Map V1 will initially have two layers: 


1. Congressional Districts
2. States 

Each layer will expose *the total number of users* and the *total number of messages* sent in respective geographic area. 

## Installation 

### Clone the repo

```
git clone git@github.com:resistbot/mapping.git
```

### Install dependencies 

```
npm install 
```

### Create a local env file and copy/paste your Rapid Pro API Key. 
```
node setup.js
```

### Create a DB in MongoDB
```
use resistmap
```

### Run the Rapid Pro data pull 
```
node bin/pull_rapidpro_data.js
```

### Start the server!
```
npm start
```
