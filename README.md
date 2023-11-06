# Introduction – Student Feedback App

As part of fulfilling the requirement of the CS7319 course we developed this application to show case Client/Server
architecture and the Layered architecture.

## Platform

### Selected Architecture

The application was developed using `python`  `version 3.10.0` programming language
and `Django framework` `version 4.2.7`.

### Downloading & Setup

1. Follow this link to download [python](https://www.python.org/downloads/).
2. Once downloaded, setup a virtual environment by running this command in the terminal `python -m venv env`,
   where `env` is the name of the environment.
3. Navigate to the folder where you created the virtual environment and run the following command.
   Windows: `env\Scripts\activate`
   Mac: `source env/bin/activate`

******NB:****** To deactivate a virtual environment navigate to the folder and run `deactivate`.

4. Once the virtual environment is activated. run the following command to install all
   dependencies. `pip install -r requirements.txt`
5. This command will spin up a local server and display the link log in the terminal. The default is `localhost:8000`

## Rationale

We chose to implement the Client/Server architecture style because this style is best suited for handling multiple
client connections. We felt this attribute would fit our requirement where multiple students (the clients) at SMU would
be using our applications at the same time.

Secondly, our choice was guided by the ease with which Client/Server can be scaled to match demand.

Thirdly, client/server architectural design is suited well for `django` since the framework uses `server side rendering`
for the `HTML` pages and all business logic is abstracted away from the client. This creates an opportunity to add more
features to our application, such as, performing analytics on review data to find the common qualms students have or
common praises for a lecturer, without being concerned about the processing power of clients.

### Unselected
FeedbackForm App

FeedbackForm application allows SMU students to provide feedback to their lectures and view them. One of the architecture styles chosen for the application is Layered Architecture Style. The implementation  of the application in a layered architecture style was done using NodeJS, ExpressJS and MongoDB.

Installation and Configuration:

1.	NodeJS - v20.9.0

Download Link: https://nodejs.org/dist/v20.9.0/node-v20.9.0-x64.msi

2.	ExpressJS - v4.18.2

3.	MongoDB Community Server - v7.0.2

Download Link: https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-7.0.2-signed.msi

Follow the Installation Steps using the below link: https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-windows/

4.	Clone git repository: 
git clone https://github.com/WilliamChavula/CS7319-Final-Project-Group-14-William-Chavula_Nashithuddin-Mohammed


Steps to Compile Code:

1.	Go to the git repository and change directory to ‘unselected’ by using the below command in the terminal.

cd unselected

2.	Run the below mentioned command in order to install the dependencies

npm install







Steps to Execute Code:

1.	Start mongoDB Server.
2.	Enter the following command in the terminal,
npm run start
3.	Open Web Browser.
4.	Go to localhost:3000 to view the app

Screenshots:

![Successful Compilation](pics/Successful%20Compilation.jpg)


![Home Page](pics/Home%20Page.jpg)

![Login Page](pics/Login%20Page.jpg)

![Register View](pics/Register%20View.jpg)

![Feedback Form View](pics/Feedback%20Form%20View-.jpg)
 

![Feedback View](pics/Feedback%20View.jpg)


## Differences
* The two architectures were implemented using different platforms. The selected was implemented using `Python language`` and the `Django Framework``. 
* The Unselected Architecture was implemented using `Javascript`` and `ExpressJS framework`. While both implementations tooks advantages of template rendering languages for the HTML pages these languages are different. Django uses a python based template language called Jinja2 while Express used the EJS template engine. 
* The selected architecture leveraged Django features in generate other UI elements (such as forms) from classes using by inheriting from Form classes in Django. 
* Another difference is that what Express calls `Controllers` which receive the `request` and `response` objects (abstractions of the web request and response), Django processes these in what are called `Views`. 