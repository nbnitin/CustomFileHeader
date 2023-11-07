# CustomFileHeader
Custom file header is the comment area which developer gets by default while adding new file. 
How to change comment area in XCode

. Create a plist or property file with name IDETemplateMacros.plist
. For every text macro you want to customize, add a new key to the plist’s dictionary. For example, to change the default file header, add an entry with the key FILEHEADER.
* Copy the file to one of the following locations. The directory specifies in which context the customized text macros should be applied:
* For a single project and user:
  * <ProjectName>.xcodeproj/xcuserdata/[username].xcuserdatad/IDETemplateMacros.plist
    * For all team members in a single project:
      * <ProjectName>.xcodeproj/xcshareddata/IDETemplateMacros.plist
    * For all projects in a workspace for a single user:
      * <WorkspaceName>.xcworkspace/xcuserdata/[username].xcuserdatad/IDETemplateMacros.plist
    * For all projects in a workspace for all team members:
      * <WorkspaceName>.xcworkspace/xcshareddata/IDETemplateMacros.plist
    * For everything you work on, regardless of project:
      * ~/Library/Developer/Xcode/UserData/IDETemplateMacros.plist

for new line in plist use option + enter

For more details
https://help.apple.com/xcode/mac/9.0/index.html?localePath=en.lproj#/dev91a7a31fc

If xcshareddata folder is not there, please create one. and it if it is added in gitignore then remove it too. it is safe to commit and push in git.



