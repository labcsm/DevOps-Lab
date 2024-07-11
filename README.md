# DevOps-Lab

                                      EXPERIMENT-1 
 
AIM: To write a code for a simple user registration form for an event. 
 
PROGRAM: 
HTML CODE: 
 
 <!DOCTYPE html> 
 <html lang="en"> 
 <head> 
    <meta charset="UTF-8"> 
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
    <title>User Registration</title> 
    <link rel="stylesheet" href="styles.css"> 
 </head> 
 <body> 
    <div class="container"> 
        <h2>User Registration</h2> 
        <form action="/submit-registration" method="post"> 
            <div class="form-field"> 
                <label for="firstname">First Name:</label> 
                <input type="text" id="firstname" name="firstname" required> 
            </div> 
            <div class="form-field"> 
                <label for="lastname">Last Name:</label> 
                <input type="text" id="lastname" name="lastname" required> 
            </div> 
            <div class="form-field"> 
                <label for="mobile">Mobile Number:</label> 
                <input type="tel" id="mobile" name="mobile" pattern="[0-9]{10}" required> 
            </div> 
            <div class="form-field"> 
                <label for="email">Email:</label> 
                <input type="email" id="email" name="email" required> 
            </div> 
            <div class="form-field"> 
                <label for="password">Password:</label> 
                <input type="password" id="password" name="password" required> 
            </div> 
            <div > 
                <input type="checkbox" id="terms" name="terms" required> 
                <label for="terms" class="terms-condition">I agree to the Terms &           
Conditions</label> 
            </div>
         <input type="submit" value="Register"> 
         </form> 
     </div> 
 </body> 
 </html> 
 
CSS CODE: 
* { 
    margin: 0; 
    padding: 0; 
    box-sizing: border-box; 
    font-family: "Poppins", sans-serif; 
} 
body { 
    min-height: 100vh; 
        display: flex; 
        align-items: center; 
        justify-content: center; 
        padding: 20px; 
        background: rgb(130, 106, 251); 
} 
.container { 
    position: relative; 
    max-width: 700px; 
    width: 100%; 
    background: #fff; 
    padding: 25px; 
    border-radius: 8px; 
    box-shadow: 0 0 15px rgba(0, 0, 0, 0.1); 
} 
h2 { 
    text-align: center; 
    margin-bottom: 20px; 
} 
form { 
    display: flex; 
    flex-direction: column; 
} 
.form-field { 
    display: flex; 
    align-items: center; 
    margin-bottom: 10px; 
} 

input[type="text"], 
input[type="email"], 
input[type="password"] { 
    flex: 2; 
    padding: 10px; 
    border: 1px solid #ccc; 
    border-radius: 4px; 
    box-sizing: border-box; 
} 
input[type="submit"] { 
    margin-top: 10px; 
    margin-left: 25%; 
    height: 45px; 
    width: 50%; 
    color: #fff; 
    align-items: center; 
    transition: all 0.2s ease; 
    background: rgb(130, 106, 251); 
} 
.terms-condition { 
    font-size: 0.9rem; 
    margin-top: 10px; 
} 
 
OUTPUT: 
 
                    EXPERIMENT-2     
  
AIM: To explore Git and Github commands. 
PROGRAM: 
1)git config: 
Usage: git config –global user.name “[name]”   
Usage: git config –global user.email “[email address]”   
This command sets the author name and email address respectively to be used with your 
commits. 
2)git init: 
Usage: git init [repository name] 
This command is used to start a new repository. 
3) git clone: 
Usage: git clone [url]   
This command is used to obtain a repository from an existing URL. 
4) git status: 
Usage: git status   
This command lists all the files that have to be committed. 
5) git add: 
Usage: git add [file]   
This command adds a file to the staging area. 
Usage: git add * 
This command adds one or more to the staging area. 
6) git commit: 
Usage: git commit -m “[ Type in the commit message]”   
This command records or snapshots the file permanently in the version history. 
7) git log:  
Usage: git log   
This command is used to list the version history for the current branch. 
8) git remote: 
Usage: git remote add [variable name] [Remote Server Link]   
This command is used to connect your local repository to the remote server. 
9)git push: 
Usage: git push [variable name] [branch]   
This command sends the branch commits to your remote repository. 

                                EXPERIMENT-3 
 
AIM: To Practice Source code management on GitHub. Experiment with the source code 
written in experiment-2. 
PROGRAM: 
1)Create a new branch: Branches in Git allow developers to work on different 
features, fixes, or experiments in isolation from the main codebase, enabling 
parallel development and efficient collaboration. 
 
  >>git branch: 
 Usage: git branch   
 This command lists all the local branches in the current repository. 
 Usage: git branch [branch name]   
 This command creates a new branch. 
 Usage: git branch -d [branch name]   
 This command deletes the feature branch. 
 
2)Switch to new branch: 
 >>git checkout: 
Usage: git checkout [branch name]   
This command is used to switch from one branch to another.
> >
3)Make the changes in the code:    
>>git diff:     
Usage: git diff   
This command shows the file differences which are not yet staged. 
 
4)Track and commit changes: 
 
5)Now merge the new branch with main branch to save changes in master 
branch: 
 >>git merge: 
Usage: git merge [branch name]   
This command merges the specified branch’s history into the current branch. 

6)Now push the changes into github repository: 
 
 
7)Now you can see the changes in your github repository: 
 

                              EXPERIMENT-4 
Aim: Jenkins installation and setup, explore the environment. 
PROCESS: 
Step-1: Download Jenkins:- 
• Go to the Jenkins website: https://www.jenkins.io/download/ 
• Click on the Windows link to download the Jenkins installer (jenkins.msi). 

Step-2: Run the Installer:- 
• Once the download is complete, locate the jenkins.msi file and double-click it to run 
the installer. 
• If prompted by User Account Control, click "Yes" to allow the installer to make 
changes to your system. 
• Follow the on-screen instructions in the Jenkins setup wizard. 

Step-3: Install Jenkins: 
• Click "Next" to proceed with the installation. 
• Choose the installation directory for Jenkins. The default directory is usually 
C:\Program Files (x86)\Jenkins. 
• The installer will begin installing Jenkins on your system. This may take a few 
moments to complete. 

Step-4:Service Login Credentials: 
• Select “Run service as Localystem” and click on “Next”. 

Step-5:Port Selection: 
• Enter a port number ex: “8080” and test port  . 
• Click “Next”. 

Step-6:Select JDK file directory: 
• Jenkins automatically detect the directory path of JDK. 
• If not then change path manually by clicking ” change ”. 
• Click “Next”. 

Step-7: Complete the Installation: 
• Click “Next ” and then click “Install”. 
• Once the installation is complete, click "Finish" to exit the installer. 

Step-8: Access Jenkins Web Interface: 
• Open a web browser and navigate to http://localhost:8080 to access the Jenkins web 
interface. 
• To obtain the initial administrator password, navigate to the location specified in the 
Jenkins setup wizard and open the initialAdminPassword file using a text editor. 
• C:\ProgramFiles(x86)\Jenkins\secrets\initialAdminPassword). 
• Copy the password from the file and paste it into the Jenkins setup wizard to unlock 
Jenkins. 



                      EXPERIMENT-5
                      
 Program 5: Demonstrate continuous integration and development using Jenkins. 
CI/CD pipeline with a GitHub repository: 
Continuous Integration (CI) and Continuous Development (CD) are 
practices in software development that aim to automate and streamline the process 
of building, testing, and deploying software.

 • Go to Dashboard click on new item and give the item a name.
 
 • Select the item as freestyle project and then click OK.
 
 • Click on Configure-> General -> Description(Give Some description.
 
 • Select discard old bills(radio buttons) 
   Strategy: Select it as  log rotation days to keep bills (14) and maximum number of  Bills to keep 20.
   
 • Select Github project -> Goto Github repository and copy the link. Go to project URL and place the Github URL in the text box.
 
 • In source Code management select git and give the Github URL.
 
 • Build Triggers select 3rd Checkbox(Build Periodically)-> Schedule, In that textbox we must give time duration  
                            TZ=IST 
                            H 21 6 * 0
                            
 Click on Save now. Click on Build now. Click on Control Output.


                               EXPERIMENT-6
 Program 6: Explore Docker commands for content management. 
Description: Docker is a popular platform that allows you to create and manage containers, which are 
lightweight, isolated environments for running applications.When it comes to content management, Docker 
provides several useful commands for efficiently managing containerised content.

 • Run command: this is used to run a container from an image by specifying the Image ID or the Repository and/
 or Tag name. 
$ docker run {image} 
e.g $ docker run nginx 
if it already exists, the command runs an instance <span class=“NormalTextRun SpellingErrorV2   
SCXW251451022 BCX0”>nginx</span> 
if it does not exist, it goes out to the docker hub (by default) and pulls the image down. 

• ps command: this command lists all running containers and some basic information aboutthem. 
$ docker ps [option] 
In option you can use various flags. To get information about the flags 
$ docker ps --help

 • ls command :like ps command, ls command can also be used for listing containers. –a flag can be used to list all 
containers. 
$ docker container ls

 • stop command: this command is used to stop a running container.After giving stop command can check with ps 
command, whether the container has stopped. 
$ docker stop {container-id}
 
 • rm command:this command removes a stopped or exited container. 
$ docker rm {CONTAINER NAME or ID}

 • exec command: this command is used to go inside a running container. This is useful to debug running 
containers or do other work within a container 
$ docker exec –it {container} {command}

 • logs command: in case acontainer is launched in detached mode and you want to see its logs, you can use logs 
command. 
$ docker logs {CONTAINER NAME or ID}

 • cp command: to copy files between a container and localhost filesystem, this command is used. 
$ docker container cp {CONTAINER NAME or ID:SRC_PATH} {DEST_PATH}|

• export command: this command exports the filesystem of a container as a TAR file. 
$ docker container export {CONTAINER NAME or ID}

 • inspect command: this command gives detailed information about a container. 
$ docker inspect {CONTAINER NAME or ID}

 • kill command: this command kills a running container with an option –signal or –s flag. Multiple containers can 
also be specified to be killed in one go. 
$ docker kill {CONTAINER NAME or ID} [--signal VAL]

                                    EXPERIMENT-7
 Program 7: Develop a simple containerised application using Docker 
Choose any application on which you want to make a container using Docker. Here the file is ‘package.json’. 
1. To begin with:
• Install Docker Desktop (Make sure you got wsl updated in your device (Win 11 / Win 
10))
   
• Install node.js (Make sure you install it with admin privileges). Check if node is 
installed using ‘npm –version’ cmd.

3. Building a node.js server application:

• Create a simple server application using node.js. 

• From a new directory, create a file called index.js. Run ‘npm init’ cmd. Check if the 
package.json and package-lock.json are added into the directory.

• Run ‘npm i express’ to install express dependency for building server.

• Write configuration code in the index.js file for a simple server. Expose a port (3000)
and an endpoint (“/”).

• Run the server application by running ‘node index.js’.

5. Check if the server is running on the exposed port from the browser by running the 
command ‘node index.js’.

6. Then, to containersie/dockerise application:

• Open docker desktop to start running the docker engine

• Go to the working directory of the server application, and run ‘docker init’ and 
specify the configuration settings

• Check if the files are added to your directory such as DockerFile, compose.yaml, 
dockerIgnore.

• Go to compose.yaml file, and configure the port mapping as per your needs 
(localPort: containerPort)

7. Running the docker container:

• Run the ‘docker compose --up build’ command. Check if the container is running in
the Docker Desktop application.

• Now visit the port you have exposed as per the config in compose.yaml. Check if the 
application is being run in your device from docker container.

8. To stop the application, run “Ctrl+C” 

                               EXPERIMENT-8

 Program 8: Install and explore Selenium for automated testing
 
 Prerequisites: Java development kit. Install Eclipse IDE for java developers. https://www.eclipse.org/downloads/ 
Download the Selenium Java client driver. https://www.selenium.dev/downloads/

 1. Install idk 17 or newer. Install Maven. Add them to environment variables.

2. Check if idk and maven are installed using “java —version” and “mvn —version”

3. Install eclipse IDE by visiting their website. Allow appropriate permissions for its installation.

4. Create a new maven project in eclipse.

5. Configure the directory, make sure to add it to project set. Proceed next.

6. Choose Quickstart archetype by apache.maven in the given list.

7. Give project details such as organisation id and archetype id (project-name).

8. You’ll have the project structure on the left side of IDE.

9. Now go to google and search for “selenium java maven dependency”. Go to maven repository url and copy the dependency code of the latest version.

10. Do the same for chrome driver java. Add the copied code, in pom.xml file in our project.
11. Write the test code in App.java file. Run the project as java application.

Code: 

“””

	WebDriver driver = new ChromeDriver();
	driver.get(“www.google.com”);
	System.out.println(driver.getTitle());
	driver.quit();

	System.out.println(“Testing completed !”);


”””
