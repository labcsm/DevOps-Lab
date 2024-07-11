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
• Create a file named dockerfile in the same folder as the file ‘package.json’ with the following contents.
 • Open a terminal and go to the ‘app’ directory with the ‘Dockerfile’. Now build the container image using the 
‘docker build’ command. 
$ docker build -t getting-started
 This command used the Dockerfile to build a new container image. You might have noticed that a lot of “layers” 
were downloaded. This is because we instructed the builder that we wanted to start from the node:12-alpine 
image. But, since we didn’t have that on our machine, that image needed to be downloaded. 
After the image was downloaded, we copied in our application and used yarn to install our application’s 
dependencies. The CMD directive specifies the default command to run when starting a container from this 
image. 
Finally, the -t flag tags our image. Think of this simply as a human-readable name for the final image. Since we 
named the image getting-started, we can refer to that image when we run a container 
The ‘.’ at the end of the docker build command tells Docker that it should look for the Dockerfile in the current 
directory.
 • Start your container using the docker run command and specify the name of the image we just created: 
$ docker run -dp 3000:3000 getting-started 
Remember the -d and -p flags? We’re running the new container in “detached” mode (in the background) 
and creating a mapping between the host’s port 3000 to the container’s port 3000. Without the port mapping, we 
wouldn’t be able to access the application.
 • After a few seconds, open your web browser to http://localhost:3000. You should see our app.
 Go ahead and add an item or two and see that it works as you expect. You can mark items as complete and 
remove items.Your frontend is successfully storing items in the backend. 
Now the Docker dashboard will show two containers running. 


                               EXPERIMENT-8

 Program 8: Install and explore Selenium for automated testing
 
 Prerequisites: Java development kit. Install Eclipse IDE for java developers. https://www.eclipse.org/downloads/ 
Download the Selenium Java client driver. https://www.selenium.dev/downloads/

 Configure Eclipse IDE with webDriver. 
Launch eclipse.exe, create a new project through File>New>Java Project. Name the project as “newproject”.
 
 Enter project name, location to save project, select an execution JRE, select layout project option, click on Finish 
button.
 Make new package as “newpackage”.
 
 Create a new Java class under newpackage by right-clicking on it and then selecting- New > Class, and then name 
it as “MyClass”. Your Eclipse IDE should look like the image below.
 Give name of the class, click on finish button.
 
After creating the class:
 
 Now selenium webdriver’s into Java Build Path. 
When you click on “Add External JARs..” It will open a pop-up window. Select the JAR files you want to add.
 
Select all files inside the lib folder.
 Select files outside lib folder.
 
 Once done, click “Apply and Close” button. 

 Add all the JAR files inside and outside the “libs” folder. Your Properties dialog should now look similar to the 
image below.
 Finally, click OK and we are done importing Selenium libraries into our project.
 
