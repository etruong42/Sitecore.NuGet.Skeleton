Sitecore NuGet Package
=================

Sitecore NuGet packages are essentially regular NuGet packages with the /tools folder full of the Powershell scripts that utilize Sitecore Rocks Hard Rock Web Service to install Sitecore files and items while also containing the full power that NuGet packages offer.

Additional folders
-----------
Sitecore NuGet packages utilize two additional folders as well as the /tools folder which you do not need to edit but can if you want to customize the NuGet experience. These two additional folders which are included in this repository are /serialization and /wwwroot. 

### /serialization
The /serialization folder will contain the serialized Sitecore items which appear at your [SitecoreDataFolder]/serialization. The serialized items that this folder contains will be installed onto the target Sitecore server. Instructions on how to serialize Sitecore items can be found at the official [Serialization Guide](http://sdn.sitecore.net/upload/sitecore6/64/serialization_guide_sc60-64-a4.pdf).

### /wwwroot
The /wwwroot folder will contain all the files which you want to be installed onto the Sitecore server. For example, if you create a file /wwwroot/bin/MyLibrary.dll, NuGet will install that file onto the target Sitecore server.

Resources
-----------
The Powershell scripts in the /tools folder originated from [a page](http://vsplugins.sitecore.net/Sitecore-NuGet.ashx) on [Sitecore's documention on Sitecore Rocks](http://vsplugins.sitecore.net/MainPage.ashx).