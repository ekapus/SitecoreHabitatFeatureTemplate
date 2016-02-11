# Sitecore Habitat Feature Visual Studio Template
There is a standard structure to Sitecore Habitat Feature Projects, and after creating a few (and blogging about it here: http://www.nttdatasitecore.com/Blog/2016/February/Building-Something-In-Habitat), I got tired of copying and renaming files. 

Because I'm a lazy programmer, I created a visual studio template to make my life, and my colleagues lives, easier. 

The src folder contains the source project that I used to create the template. The Sitecore Habitat Feature Visual Studio Template.zip file contains the template that can be installed in visual studio.

##Feature Project Template Installation Instructions
1. Download Sitecore Habitat Feature Visual Studio Project.zip from https://github.com/ekapus/SitecoreHabitatFeatureTemplate
1. Copy the zip file to to \My Documents\Visual Studio Version\Templates\ProjectTemplates\Language\ on your local machine.
1. Run the following command from the Visual Studio Command Line (accessed from the start menu at Visual Studio 2015/Developer Command Prompt For Visual Studio 2015:
```
devenv /installvstemplates
```
_Note: this can be done while Visual Studio is running._

For more info about finding, organizing and installing Visual Studio Project Templates: https://msdn.microsoft.com/en-us/library/y3kkate1.aspx


##Feature Project Template Use Instructions
1. Create a new solution folder in your Habitat Solution under "Feature" that describes your feature.
1. Right click on the new solution folder, choose add, and select "New Project".
1. Scroll through the project types and select "Sitecore Habitat Feature".
1. Enter a name for your feature. It's best to omit spaces and punctuation.
1. Using windows explorer, create a folder that matches your solution folder name under "Your Habitat Project Root\src\Feature"
1. Under the folder you just created, create a "code" and a "serialization" folder.
1. Choose the code folder as the location for the project you're creating.
1. Hit OK
1. Open your new project.
1. Rename /Views/$safeprojectname$ to /Views/YourProjectName
1. Rename /Models/$safeprojectname$ to /Models/YourProjectName