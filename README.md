# React Chat App

This repo shows how to easily add chat functionality into a NodeJS project with [Chat Engine](https://chatengine.io).
This project enables users to have their own chat application with many features like read recipients, sending files, photos and videos, Group chat, etc.

## Setup Steps
Make your own simple chat application - in 3 steps:

### 1 - Setup a Chat Engine server

Go to [Chat Engine](https://chatengine.io) to setup your own chat server.
- Click "New Project" and follow the steps
- Your `Project ID` and `Private Key` will be required for step 2

### 2 - Connect `.env` to Chat Engine

We will connect to your Chat Engine server with environment varibles.
This allows you to connect to different chat-servers in local vs staging vs production.
Replace the UUIDs below with your own. In the `server/` `.env` write:

```
CHAT_ENGINE_PROJECT_ID=5d498a31-cd23-42b7-b367-4fcc9463bd2f
CHAT_ENGINE_PRIVATE_KEY=49a46286-91c3-4f9c-92bf-284ae51b7628
```
Replace the UUIDs below with your own. In the `client/` `.env` write:
```
REACT_APP_CHAT_ENGINE_PROJECT_ID=5d498a31-cd23-42b7-b367-4fcc9463bd2f
```
### 3 - Install & Start

Run the following two lines of code in `server/`.
```
npm install
npm run start
```
Run the following commands in `client/`.
```
npm install
npm run start
```
Done! Your chat application is on `localhost:3000` and connected to Chat Engine!
All new `/signup` users are on Chat Engine, and their credentiuals are found upon `/login`.

