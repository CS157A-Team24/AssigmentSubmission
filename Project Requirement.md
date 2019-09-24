<h1 align="center">
    <br>
    <br>
    SeenIT  
    <br>
    <br>
</h1>

<h3 align="center">
    by
    <br>
    <br>
</h3>
<h2 align="center">
    Chaz Chang
    <br>
    Viet Dinh
    <br>
    My Nguyen
    <br>
    <br>
    TEAM 24
    <br>
    CS157A
</h2>

<p align="center">
  <a href="#project-overview">Project Description</a> •
  <a href="#system-enviroment">System Enviroment</a> •
  <a href="#functional-requirements">Functional Requirements</a> •
  <a href="#non-functional-issues">Non-functional Issues</a>
</p>

## Project Description

### Overview:
The goal of this application is to create social news, rating site, and discussion website. Users can be able to check daily news, search, filter, and sort through posts. Also, users can create posts, comment on them, like, and share posts. In addition, users can create channels that will function as communities. Users can view posts without logging in, but creating posts, commenting, and liking will require the user to login. This application will allow people to easily voice their opinion or share a story. People can easily ask questions and others can answer them. It will also provide a user-friendly interface and fast response time while maintaining high throughput. 

### Who would be interested in this application?
Users could be anyone who is interested in forming a community online, and interact with people with similar interests. Users can keep up to date with news, information, and ideas in their community. Companies and organizations can use Seenit to communicate with people and market products.

## System Enviroment

#### Structure of the system (graph based on 3-tiered architecture):
*INSERT DRAWIO PICTURE*

#### HW/SW used:
+ ReactJS
+ NGINX
+ Spring Boot
+ Windows/macOS
+ MySQL Workbench
+ Visual Studio Code

#### RDBMS Used:
+ MySQL Version 5.6

#### Application languages:
+ Java (with Spring Boot framework)
+ SQL (with MySQL)
+ JavaScript (with ReactJS)

## Functional Requirements

### How users will interact with the system:
The application provides the same functionality for all the users. Internet connection is required for any activity on the system. A user shall be able to access the system for read and write. A user can access the system home page freely. They shall be able to read daily news and posts from various websites without logging in. Users can also be able to make a search based on their particular interests. However, users must log-in into the system and have their credentials checked for other activities such as make a new post, comment on a post, share a post, create a sub-channel, and follow another channel. Especially, first-time users must register for an account to perform the activities listed above under log-in. 

### Describe each individual function, functional process and I/O:

### Functions:

#### Log-in
+ Returning users must sign-in to perform the following activities: 
	+ create or access personal channel
	+ add a new post
	+ like or comment on someone else's posts
	+ share a post
	+ follow another subchannel
	+ delete personal posts
+ Guests or unregister users can only view posts
+ The system shall check the users' credentials. If the entered information does not match the data stored in database, an error message will be displayed; for instance, "ID or password is invalid." The users can either create a new account or reset password/username. Otherwise, the system gives users access when the data matches.

#### Register for an account
+ There will be only one type of user; no admin account in this application. First time user must sign up for an account to perform those activities listed in log-in function
+ There will be a redirect link. User will be asked to fill out some information such as first name, last name, email address, username, and password. 
+ No limitation. Users can set up multiple accounts and choose which one to log-in with depending on the personal channel which users want to participate in. 
+ The system shall check if the entered username is already existed. The system shall keep asking the users to enter a username until the name is available. Then, the system shall add the users' personal information into database.

#### Reset
+ The users shall be able to reset password or username when they forget it.
+ The system will send a verification code via the user's email. 
+ The users must check the provided email for verification code, and then enter the code to the verification code box to reset username or password. Users must request for a new code if they do not see it. 
+ The system shall verify the code. If the code is correct, the system will update the database after the users finish submitting new information. 

#### Create a sub-channel 
+ Once users are signed in, users can create their own channels (similar to social media accounts). On their channel, users can be able to manage role of other users, make a new post, delete a post, check out subcribers, and display personal dashboard.
+ Users can create multiple sub-channels (up to 4). By creating a subchannel, a user can get followers or subscribers who are interested in his/her activities.
+ The system shall save information of the sub-channel in database.

#### Search 
+ The users shall be able to search for daily news and posts by typing in keywords which appear in titles or headlines in search box. The users can also be able to search for a subchannel by entering the name of that channel in a search box.
+ If there is no matching results, the system shall display a message to indicate that whatever the users are looking for was not found. Otherwise, the system display all the posts or news which are related to the searched terms.

#### Add a post

#### Commenting
+ The users shall be able to leave multiple comments on someone else's posts by click on the comment button, type what they want to say in the reply box, and hit enter. 
+ Once a comment is submitted , the data will be saved to the associated subchannel. They can later check which posts they commented on the subchannel dashboard.

#### Share a post
+ When users are interested in a particular post, or they think a post is useful for other people, they can be able to share that post. To share a particular post, the users must click on the share button under a post. The shared post will be automatically added to their sub-channel, and others shall be able to view or share it.
+ By sharing a post, the users can always go to their sub-channel to continue reading it if they do not have time to fishing reading the post at once.

#### Edit

#### Delete

#### Follow a specific user

#### Display personal dashboard

#### Display other users' dashboard

#### Filter

#### Sort


## Non-functional Issues
### Graphical User Interface (GUI): 
There are many design principles when it comes to web design. 
### Security
### Access Control
+ Anyone with internet can access the website
+ A user will be able to view posts and channels without logging in
+ A user must login to create posts, comments, or channels
+ A user cannot edit posts or comments that belong to a different user
### Performance
+ Fast response time while maintaining high throughput
### Scalability
+ Able to add new functions and features while developing the app

