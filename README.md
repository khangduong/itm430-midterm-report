# ITMT 430 
# Team 5 Octocat - Sprint One Report
# InterpretAir Project

##### Team Members
1. Alex Wang
2. Aury-Ken Bwashi
3. David Powers
4. Khang Duong

---

#### Project Name and Concept
Our project is called InterpretAir and it is going to be a web application that uses real-time video translation.
The goal is to improve the communication quality between people who don’t speak the same language by utilizing existing technologies (i.e. Amazon Transcribe, Google Translate, Vidyo) in the form of API's and building our own product.

#### Scope
This project is a web-based Real Time Communication platform used to transcribe and translate communication remotely between users who don't speak the same language. The project duration is 16 weeks starting from January 9th until April 22nd. Features that will be implemented in this time frame will be video call between two or more users (video conference/group call up to 6 users). Transcribing the video call conversations and translating the transcripts to the desired language by the user - this feature will only be implemented between two users due to the time constraint. The transcripts will be saved if the user is signed up and has an account with InterpretAir. All personal information and password will be protected using database encryption and password hashing. 

---

### Industry Competitors
There are a lot of competitors out there that provide voice over IP services so these industry competitors were chosen due to the similar functionalities that they offer and the same target market. These services are the most popular ones out of the bunch and they are trying to solve similar problems that we are trying to solve.  

#### Skype/Skype Translate
##### How do they function:
Skype is a proprietary VoIP system using its own protocol based on peer-to-peer (P2P) networking; essentially, it works by creating ad-hoc, direct communication between two computers on the Internet. When you sign on to Skype, your computer becomes one node in a global network of equal peers. Each Skype user runs a piece of software called a client that allows them to send messages to other Skype users, make calls, send files, and play real-time games. Each of the clients becomes an active part of the network and, whether it's actively sending messages or not, helps the network as a whole to locate and route traffic to other users. Within the network, some of the users with highest bandwidth and best connectivity, known as supernodes, act as traffic hubs. The network as a whole is made up of supernodes connected to one another, with each supernode linking to many ordinary nodes.

Skype Translate takes the words you speak, converts them into text, translates that text, and then synthesizes them into spoken words in the language of the person on the other end of the call. 

##### How are they built:
The "core" functionality - making audio, video and messaging, so the shared business logic - are written in C++ and built targeting the specific platform. The Windows Skype desktop client is written mostly in Delphi, using the mentioned C++ component for the core business logic. The mobile versions are written in the native language those platforms support, so the iOS client is written in Objective C, Android in Java, Windows Phone in C#. The mobile versions use similar, but mobile optimized C++ libraries to the desktop for the core calling functions.  The other platforms - Mac, XBox, Sony Smart TV etc - all use the native development language for the given platform and similar C++ libraries.

Skype Translator uses machine learning. So the more you use it, the better it gets. Their voice translator currently works in 8 languages, and our text translator is available in more than 50 languages for instant messaging.

#### Google Hangouts
##### How do they function:
Google Hangouts is a communication platform developed by Google which includes messaging, video chat, SMS and VOIP features. Hangouts allows conversations between two or more users. The service can be accessed online through the Gmail or Google+ websites, or through mobile apps available for Android and iOS. Chat histories are saved online, allowing them to be synced between devices. Google+ Hangouts users can also perform a group video chat with up to 10 users at a time. It replaces three messaging products that Google had implemented concurrently within its services, including Google Talk, Google+ Messenger, and Hangouts, a video chat system present within Google+. 

Google is splitting Hangouts into two: Hangouts Chat, which is clearly gunning for Slack, and Hangouts Meet, which is all about video and audio communications. Those two are basically the enterprise counterparts to Allo and Duo.

##### How are they built:
There are not many current information about their current technology stack, but for 
Google Talk (2011): The client was written in C++. The service is written in Java. 
Google+ (2011): 
1. Java servlets (for  server code)
2. JavaScript (for the browser-side of the UI)
3. Closure framework (as template system)
4. HTML5 History API (to maintain pretty-looking URLs)
5. BigTable and Colossus/GFS (on top of which the backends are built)
6. MapReduce

Google Talk and Hangouts had used technology Google is licensing from Vidyo to facilitate video chats just like we are using for our web application. However they switched to open codec like Skype. 

#### Appear.in
##### How do they function:
Appear.in is a video collaboration tool that lets you have video conversations. The PRO package supports up to 12 people simultaneously. You can create a room with no required registration. The user can upgrade the room to PRO to customize it and for more great features. 

##### How are they built:
This one is not quite popular and we couldn't find out which technology stack it's built in. Our best guess is Javascript for the client side and not sure about the server side. 

---

### Roles 
| Roles            | Sprint 1           | Sprint 2           |  Sprint 3                         |
| -------------    |--------------------| -------------------|-----------------------------------|
| Project Manager  | Marika Jasinski    | Alex Wang          | Khang Duong                       |
| Developer        | Aury-Ken Bwashi    | Khang Duong        | David Powers                      |
| Junior Developer | Khang Duong        | Aury-Ken Bwashi    | David Powers/Aury-Ken Bwashi      |
| UI/UX            | Alex Wang          | David Powers       | Aury-Ken Bwashi                   |
| IT Operations    | David Powers       | Marika Jasinski    | Alex Wang                         |

---

## Goals

### Sprint 1
In the Sprint 1, we divided the project into different parts which we agreed, as a team, that they consist of the most critical functions of the project. We prioritized the functions of the web application and we thought we should tackle the main functions first as they are the most time consuming. The main functions include Vidyo.io API, Transcribe and Translate. We chose to create a skeleton of the project first, then create the "empty" web pages (profile, contacts, settings) without any functionalities to have a visualised flow of the website. At the same time, IT Operations role was starting to create a shared environment using Vagrant, Packer and VirtualBox. Project Manager was responsible to create an efficient system by dividing the tasks to Trello cards and using Slack to check on the work of each role. 

| Goals                                                                                                   | Status             |
| --------------------------------------------------------------------------------------------------------|:------------------:| 
| Generate Deploy keys                                                                                    | Completed          | 
| Create/Design profile, contacts, and settings web pages                                                 | Completed          | 
| Create logout action                                                                                    | Completed          | 
| Refine the UI Layout Design                                                                             | Completed          | 
| User signup with mongoDB                                                                                | In Progress 35%    | 
| Demo a Vidyo.io call                                                                                    | In Progress        | 
| Integrate Authentication                                                                                | In Progress        | 
| Translation | Transcribe                                                                                | In Progress        | 
| Intergrate vagrant/packer automation                                                                    | In Progress        |
| Extract audio from Video                                                                                | In Progress        |



### Sprint 2
Since, our goals for first week
| Goals                                                                                                   | 
| --------------------------------------------------------------------------------------------------------|
| Generat Deploykeys                                                                                      |  
| Create/Design profile, contacts, and settings web pages                                                 | Completed          | 
| Create logout action                                                                                    | Completed          | 
| Refine the UI Layout Design                                                                             | Completed          | 
| User signup with mongoDB                                                                                | In Progress 35%    | 
| Demo a Vidyo.io call                                                                                    | In Progress        | 
| Authentication Integration                                                                              | In Progress        | 
| Translation | Transcribe                                                                                | In Progress        | 
| Intergrate vagrant/packer automation                                                                    | In Progress        |


### Sprint 3
| Goals                                                                                            | Status           |
| -------------------------------------------------------------------------------------------------|------------------| 
| Review/Modify Milestones according to new artifacts                                              | Completed        | 
| Integrate Vagrant and Packer: (same deployment environment with MongoDB running)                 | In Progress: 90% | 
| Integrate Vidyo call                                                                             | In Progress: 80% | 
| Complete signup with MongoDB                                                                     | In Progress: 60% | 
| Dynamic logged in and unauthenticated pages                                                      | In Progress: 40% | 
| Intergrate Transcribe && Translation                                                             | In Progress: 30% | 



# 13 Base Project Requirements
Why did you choose them? What do they do? What do they allow you to do?


### 1. MEAN Stack
MEAN is an acronym, which stands for Mongo DB (database system), Express (back-end web framework), Angular.js (front-end framework) and Node.js (back-end runtime environment). Our team is the most comfortable with Javascript and it is a modern approach to web development. JavaScript is a dynamic programming language for client-side and server-side web application development.

MEAN stack uses JSON as the format for data-interchange on all the layers. So, there is no need to use libraries for converting data during client-side and server-side interaction. JSON also allows working with external APIs (application programming interfaces) easily which is ideal for our project.

Mongo DB is a great choice for database system when managing huge tables with tons of data. Unlike any other database, adding a field to Mongo DB is simpler as it does not require updating the entire table. Moreover, it is a NOSQL and a document model database, which is extremely flexible to use in a variety of applications. In Mongo DB, documents resemble to objects in an object-oriented programming language. A document can be queried on any field and data access is simplified by reducing the use for joins.

Express.js is used in creating server side web applications faster and smarter, simplicity, minimalism, flexibility, scalability, easy to configure and customize, allows you to create rest API server, easy to connect with databases.

Angular.js is a front-end JavaScript development framework for developing single-page applications. It allows a clean way of adding interactive functions and AJAX-driven rich components on the client-side. Since, you have Node.js providing a server-side solution; there is JavaScript implementation on both client and server-side. This makes programming applications with MEAN stack very effective.

Node.js also runs on LINUX, Windows and OS X. Node.js operates on a single thread for processing incoming HTTP requests. It uses non-blocking I/O (input-output) calls to handle multiple new incoming requests efficiently. Unlike other web servers like Apache, Node.js is extremely fast and scalable, supporting thousands of concurrent connections. Node.js uses web sockets to enable sending data to client without having the client to request it. Hence, it is an ideal choice for developing real-time web applications like chatting applications. Node.js is also supported by a large module library. 
 
### 2. Operating System: Ubuntu Linux Distribution

### 3. MongoDB used to store data.
### 4. Data encrypted at rest
Passwords are hashed to protect personal information. Private networks are only being used by admin.
### 5. Database Master/Slave Replication
### 6. Use of Responsive Design 
Make sure login and signup are resizable and work cross platforms both on the website and mobile phones. 
### 7. Use of https
Make sure the communication is secured and protected. Real Time Communication. 
#### a. Self-signed certs 
#### b. Google Authentication for login
Using Gmail to login. 
#### c. SQRL
### 8. Use of user authentication
Unathenticated users can use the platform without logging in, by just creating a room and inviting other users in. Transcripts are not stored in their account but end of each call, there will be a summary page with the option to download or email the transcript to themselves. 

Authenticated users will have their own account where they can store their transcripts and have a list of contacts. The list of contacts allows the user to chat or call them when they are online. 

### 9. Creation of Dev Environment (local laptop)
Most of our configurations are done by scripts under provisioners in our VagrantFile.  

### 10. Layout Design
Layout design is simple and user friendly. Not cluttered, it will be minimal but still with all the required functionalityies. 

### 11. Management of Visio
Created diagrams of User workflow and Application architecture
Application Architecture of MEAN stack and MVC infrastructure. 

### 12. Management of Project progress
1. Trello
These cards help us stay on top of our tasks and see what everyone is doing. The cards hold us accountable and responsible for different tasks. If someone runs into a problem, they can ask for help or assistance on slack or in weekly meetings. 

2. Slack
Slack is used extensively to communicate and chat about our progress and problems. Share technologies that could be implemented in our project and see what is feasible. 

Snippetbot - atomic goals metric

3. Github
This is where our entire code is hosted on. We can see who 

4. Github Issues to resolve bug posts from UI/UX tester

### 13. 15 real "test" users and proper data to test functionality of a system - No system is ever used "blank" always fill it up with real data
Users accounts are stored in the database server after the user inputs their personal information in the registration form. There are 15 test users that can login to the authenticated site which allows them use the main functionalities and store transcripts after phone call. 
 
 
## Sources 
https://www.quora.com/What-is-Skype-coded-in
http://www.explainthatstuff.com/how-voip-works.html
https://www.wired.com/2014/12/skype-used-ai-build-amazing-new-language-translator/
https://www.skype.com/en/features/skype-translator/
https://blogs.skype.com/news/2014/12/15/skype-translator-how-it-works/
https://www.quora.com/What-are-the-programming-languages-used-in-making-Google+
https://www.quora.com/What-language-is-Google-Talk-written-in


