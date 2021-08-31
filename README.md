# Transcript Generation in Video Call
Hey Code geek, welcome to my project 'Transcript generate in video call'. It was a great journey to build such great project with everyone. We beleived that many deaf people require engagement in these video calls , so my feature will defenitely help in it. Apart from this , it can also be used as minutes of the meeting.
<br/>
Challenge was basically about generating transcript and connecting two people on teams via video calling. On above of that I incorporated following features:
* [Join or Create Room](#create-room)
* [Group Video Calling](#meeting)
* [Meeting Chat (inside meeting)](#meeting-chats)
* [Teams Chat (outside meeting)](#teams-chats)
* [Screen Share](#screen-share)
* [Screen Recording](#screen-recorder)
* [Transcript](#transcript)
* [Authorization](#sign-in)

**Website Link**: [teams-clone-shashwat](https://teams-clone-shashwat-sahu.web.app)

**Youtube Link:**: [Transcript generation in Video call](https://youtu.be/8iSFCWuq1no)

***Thanks to [symbl.ai](https://platform.symbl.ai/#/home) for Live Speech to Text API*** 

# Tech Stack
* React.js
* Symbl.ai
* Node.js
* MongoDB
* WebRTC

were used to build this project.
# Steps to Access
**Important**
<br/>
* Please get MONGO URI from mongodb and paste it into .env as 
<br/>
MONGO = "uri token"
* Please get app Id and app secret from symbl.ai and paste it into .env as
<br/>
appId = "token"
<br/>
appSecret = "token"

<br/>

**To Join Meeting**
<br/>


Step 1: Sign Up on website and then login.
<br/>
Step 2: Create Room with name (optional) or join room by either pasting url in browser or using room ID.
<br/>
Step 3: Chat with people in room and connect.
<br/>
Step 4: Click on Join meeting icon and it will redirect you to meeting.
<br/>
Step 5: Connect with people on meeting

**To enable Transcript**
<br/>
Step 1: Click on enable transcript option under 3 dots.
<br/>
Step 2: Open transcript panel to see live speech to text , though will be visible infront as well.

**To Start Screen Sharing**
<br/>
Click on screen share option and it will enable it to everyone in the meeting.

**To Record Screen**
<br/>
Step 1: Click on start screen recording under 3 dots (only possible when screen sharing is already on).
<br/>
Step 2: Stop screen recording by clicking on "Stop screen recording" to save file locally on your device.

# Agile Implementation
The Development was a series of continuous Integration and continuous Deployment. Each functionality was divided in weeks under SCRUM.  Each sprint’s goal was to build the most important features first and come out with a potentially deliverable product. Testing was done on Selenium IDE. Also even adapt feature which is taken as customer needs, was added in subsequent sprint.
<br/>
Priorty Level:
* 1: Lowest Priority
* 2: Low Priority
* 3: Medium Priority
* 4: High Priority
* 5: Highest Priority


|Type|Week|Description|Priority level|Status
|----|----|-----|-----|-----|
Setup|Week 1|Front End : React<br/>Backend: Nodejs<br/>DBMS: MongoDB| 4|Completed
Feature|Week 1|Video Calling between two people| 5|Completed
|Bug 01| Week 1| Peer Connections disrupted| 5|Resolved
Feature|Week 1|Video Calling between group of people| 4|Pending
|Bug 02| Week 1| Peers not destroying in group video calling| 5|Pending
Feature|Week 2|Meeting Chat| 3|Completed
|Bug 02| Week 2| Peers not destroying in group video calling| 5|Resolved
Feature|Week 2|Video Calling between group of people| 4|Completed
Feature|Week 2|Screen Sharing| 3|Completed
Feature|Week 2|Meeting Chat| 3|Completed
Bug 03|Week 2|Scren Sharing not enabled for other people|5| Resolved
Feature| Week 3| Screen Recording|3 |Completed
Feature| Week 3| Transcript Added (Socket implementation remaining)| 2|Pending
Feature|Week 4| Chat outside meeting (Adapt feature)|5|Completed
Feature|Week 4|Authorization|3|Completed
Feature| Week 4| Transcript Added (Socket implementation)| 2|Completed
Procedure|Week 4|Testing Phase (on selenium IDE)|3|Completed
Procedure|Week 4|Code cleaning|2|Completed

# Pre Requisites
* Gain Mongo access link from from Mongo DB and paste in .env as MONGO_URI
* Gain App id and access token from symbl.ai and paste in .env as 'appid' and 'accessToken'

# Client Side
## Code Prospects
### `npm install`
Install modules mentioned in package.json
### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.


# Server Side
### `npm install`
Install modules mentioned in package.json
### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:8000](http://localhost:8000) to run server.

You will also see any errors or information in the console.
# E-R Diagram
![er](https://raw.githubusercontent.com/Shashwat-Sahu/microsoft-teams-assets/main/Picture1.png) 

# Flow of functionalities
## Group Video Call 
<img src="https://raw.githubusercontent.com/Shashwat-Sahu/microsoft-teams-assets/main/Picture2.png" alt="video-call" width="450"/>

## Screen share
<img src="https://raw.githubusercontent.com/Shashwat-Sahu/microsoft-teams-assets/main/Picture3.png" alt="screen-share-diagram" width="450"/>

# Screenshots

## Sign In
![signin](https://raw.githubusercontent.com/Shashwat-Sahu/microsoft-teams-assets/main/signin.png)

## Sign Up
![signup](https://raw.githubusercontent.com/Shashwat-Sahu/microsoft-teams-assets/main/signup.png)

## Teams Chats
![teams chats](https://raw.githubusercontent.com/Shashwat-Sahu/microsoft-teams-assets/main/Screenshot%202021-07-11%20195107.png)

## Create Room
![create room](https://raw.githubusercontent.com/Shashwat-Sahu/microsoft-teams-assets/main/create%20room.png)

## Join Room
![join room](https://raw.githubusercontent.com/Shashwat-Sahu/microsoft-teams-assets/main/join%20room.png)

## Home
![home before joining](https://raw.githubusercontent.com/Shashwat-Sahu/microsoft-teams-assets/main/web%20home.png)

## Meeting
![meeting](https://raw.githubusercontent.com/Shashwat-Sahu/microsoft-teams-assets/main/web%20meet.png)

## Transcript
![transcript](https://github.com/Shashwat-Sahu/microsoft-teams-assets/blob/main/transcript.png?raw=true)

## Meeting chats
![meeting Chats](https://raw.githubusercontent.com/Shashwat-Sahu/microsoft-teams-assets/main/web%20chat.png)

## Screen Share
![screen share](https://raw.githubusercontent.com/Shashwat-Sahu/microsoft-teams-assets/main/web%20screen%20share.png)

## Screen Recorder
![meeting Chats](https://raw.githubusercontent.com/Shashwat-Sahu/microsoft-teams-assets/main/web%20screen%20recorder.png)

### Screen Recorder Example
![meeting Chats](https://github.com/Shashwat-Sahu/microsoft-teams-assets/blob/main/recording.gif?raw=true)


