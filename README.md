# Auto generate Package.xml using ANT and Metadata API

Auto generate Package.xml file using ANT Script. Get All Folder and file names in Package.xml

**Prerequisite:**
* Force.com Migration Tool [Read how to download](http://www.salesforce.com/us/developer/docs/daas/Content/forcemigrationtool_install.htm)
* AntContrib [download from here](http://mvnrepository.com/artifact/ant-contrib/ant-contrib/1.0b3)

 [![Salesforce – Auto generate Package.xml using ANT and Metadata API](http://img.youtube.com/vi/CPMLkX4ewuk/0.jpg)](https://www.youtube.com/watch?v=CPMLkX4ewuk)

**How to Execute:**
* update "build.properties" with correct username, password, and server url
* Place Force.com Migration Tool JAR file in root of this directory
* Folder will look like this, ![Directory after initial setup](/img/postSetupDirectory.png)
* Open Command prompt
* Navigate to folder where "build.xml" is present. This will create a package.xml file in the tmp directory.
*  execute command : `Ant` or `Ant testPackageXML`
* Once executed, copy the package.xml file from /tmp to /codepkg

Now retrieve the actual metadata from your org
* execute command : `ant -f sfmigration-build.xml retrieveCode`
* command will run and provide status updates via command prompt until complete