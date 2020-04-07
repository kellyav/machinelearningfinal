# Beginers Guide to posting code (manually) on Github:

You can do this one of two ways. Manually on the website or through a push request using Terminal (Command line) code. 
  It is more challneging to do it the manual way, but this guide is an attempt to explain how to go about it.

*See: https://github.com/kellyav/isat_2020/blob/master/git_upload_guide.md for my Commandline How-to guide.*


Start by navigating to the main page of the repository on GitHub.

## To update changes to our R markdown file: 
*note that you can edit the code directly on Githubs website 
but I doubt we will actually do that so* here is how to update the repository with changes to the Rmarkdown file:

1. Download this repository so that there is a copy on your computer. To do this, click "clone or download"

2. Click "download zip" This will not actually download as a zip file, but now the folder will be saved on your computer. 
Edit the R markdown file like you normally would and save that same file so that it is changed within the folder. 

3. We will have a "development" branch. This will be where all the version history changes will be made. 
*You can also create and use your own branch you can update if that suits you better.*

Do this by clicking "Branch: ----" and clicking on development. 
When a change is made, these changes are saved as _commits._

Each time you commit it is a good idea to add a short commit description, to create a readable history of the project, 
and it allows contributors to understand what is going on at a glance.
Changes done to our development branch will stay there until we update the master branch.

*Note: if you commit directly to the master branch instead of doing the above, 
it will completely overwrite the old versions of the code.*


4. To update the master branch, we need to 'pull' the updates from the development branch into the master branch 
- this is done by doing a **Pull Request**.

5. So to open a Pull Request for the changes done to the markdown file, click the tab (located next to 'issues' and 'actions').
Select the green New pull request button.

6. The base should be set to master and the compare should say development. write a description of your changes.

7. A Pull Request needs to be 'reviewed' before the changes are merged, 
basically to double check that what is about to be merged is actually what you want it to be.

It will highlight the differences in the content between branches. 
Changes can be additions or removal of the content. 
Additions are highlighted in green, and subtractions are highlighted in red.


8. Click merge pull request and it will be updated!


## To add a completely new file: 
1. Under your repository name, click Upload files.

2. Drag and drop the file or folder you'd like to upload to your repository onto the file tree.

3. At the bottom of the page, type a commit message that explains the change you made to the R markdown file. 

The commit will post with your name on it, saying that you made changes and when the last changes were made. 

**! Important !** For us, since we are working with three people and the project will consist of a lot of moving parts, 
choose the "Create new branch" option when posting the code. That way we can create a version history and it doesnt replace older version of the code, just in case something goes wrong like an error, and we can go back and look at previous versions.
Name the branch by version number and keep the naming consistent. 

4. Click Commit change/ propose file change.

5. This prompts the page to Open a Pull Request. You can leave further comments here if you want to. 

6. Then click Merge Pull Request.  

7. Click Confirm merge and voila!
