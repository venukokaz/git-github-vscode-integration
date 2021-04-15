# git-github-vscode-integration
How to integrate Git, GitHub in Visual Studio Code

Covered
I.Adding a new project to Git & GitHub
II.Pushing new changes to Git & GitHub
III.Cloning an existing GitHub repo to our local computer (Step 11)
IV.Removing project from Git (Step 12)

1.Install Git(version > 2.0.0) in your system (local computer) - https://git-scm.com/downloads
    Note: VS Code will leverage your machines Git installation

2.Check current Git Installation in your system (Win,macOS)
    $git --version
     
3.Create an account in GitHub - https://github.com

4.Create a new repository in GitHub - <DemoApp>

5.Copy the URL(HTTPS) of the Repo :  <https://github.com/venukokaz/DemoApp.git>

6.Verify if Git is Enabled in VS Code Settings : Ensure it is checked as shown in the picture
   On Windows : Open VS Code -> File -> Preferences -> Settings -> Search for 'git enabled'
   On macOS   : Open VS Code -> Code -> Preferences -> Settings -> Search for 'git enabled'
 
   <img src='images/git-enabled-vscode.PNG' width=600>

7.To integrate with Git (On local) :
  Goto VS Code -> File -> Open Project directory(that you want to upload to GitHub) -> Click on Source control icon  on left panel ->
  Click on Git Icon -> Initialize a repository -> Unstaged Status -> Enter a commit message & Commit changes [On Win :  Ctrl + Enter]
  
8.To push to GitHub (Remote) :
  Goto VS Code -> Click on Source control icon  on left panel ->  View -> Command Palette -> Type in "add remote"  -> 
  -> Provide Git URL : <https://github.com/venukokaz/DemoApp.git>  -> ...  -> Push 
  
9.Verify in GitHub Web interface whether files are uploaded or not.

10.For new changes -> VS Code auto detects the changes we make in our files -> Add message and push whenever needed

11.To clone a repository & bring it to local 
   Goto VS Code -> New -> Ensure git is enabled (Refer Step 6) -> Click Source control icon on left panel -> View -> Command Palette ->
   -> Type "clone" ->  Provide Git URL : <https://github.com/venukokaz/DemoApp.git>  -> Choose a directory of your choice 

12.To remove project from Git
   Goto VS Code -> File -> Open Project directory -> View -> Command Palette -> Type : "close repo" 
   +
   Manually delete .git folder from project directory

References :
a. VS Code documentation on Version Control :  https://code.visualstudio.com/docs/editor/versioncontrol
 


