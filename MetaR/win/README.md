![MetaR logo](../images/MetaR-logo-4-SMALL-300x111.png)

## Installation instructions for Windows users

**NOTE:**

Support on Windows is still experimental and under active development. Even if most of the features work, there are a few issues to fix that can affect the correct execution of the Analyses. 

System requirements
-
[MetaR](https://manuelesimi.github.io/MetaR/) can be installed only if these requirements are met:
* 64bit Windows 10 Pro, Enterprise and Education (1607 Anniversary Update, Build 14393 or later)
* about 4GB of disk space available.

Install software required by MetaR
-
1. Open the Command Prompt (Start button > All Programs > Accessories > Command Prompt) and type:
   java -version
   If the version is less than 1.8.0, download and install the Java 8 Environment from
   https://java.com/en/download/
    
2. Download and install Jetbrains MPS 2019.1.5 from [http://download.jetbrains.com/mps/2019.1/MPS-2019.1.5.exe](http://download.jetbrains.com/mps/2019.1/MPS-2019.1.5.exe)

3. Install R from [https://cran.r-project.org/bin/windows/base/](https://cran.r-project.org/bin/windows/base/) and then run this [R script](R-installation.R.txt) inside the R console to install some R packages required by MetaR
   
Install MetaR
-    
1. Install the MPS metaR plugin
    
    1.1 Start the MPS application and open-up the plugin manager in MPS (menu File > Settings… > Plugins)
    
    1.2 Click on the gear icon (top righ) and then select “Manage Plugin Repositories…” button.
    
    1.3 In the new window ("Custom Plugin Repositories", then + (plus) button, add the following URL: http://mpsrepo.slisson.de/ and then click OK
  
    ![Repo](../images/AddRepoURL2019.1.png){:height="50%" width="50%"}
    
2. Back on the “Plugins” window, click on "Marketplace" and search for "MetaR" and click on the install button of the plugin _org.campagnelab.MetaR_. Restart the application to activate the plugin.
  
    ![PluginInstall](../images/InstallMetaR2019.1.png){:height="50%" width="50%"}
    
3. After restarting, open MPS, go back in the plugin manager (menu File > Settings… > Plugins) and make sure the MetaR plugin is not listed red.

   ![PluginCheck](../images/CheckMetaR2019.1.png){:height="60%" width="60%"}

Configuration
-    

1. Define the following Path Variables (menu File&gt;Settings...&gt;Appearance &amp; Behavior&gt;Path Variables):
    * **Name**: _org.campagnelab.metaR.results_dir_
    * **Value**: an arbitrary folder <strong>under C:\Users\ </strong>where you want the results of MetaR analyses to be placed. (**Avoid a path with spaces.**)
  
    ![AddVariable](../images/AddVariable.png){:height="80%" width="80%"}

2. Define the following Path Variable (menu File>Settings…>Appearance & Behavior>Path Variables):

    * **Name**: _R_HOME_
    * **Value**: _installation path to R_ (where R has been installed)

   Calling R.home() in the R console will return the installation path. See https://stat.ethz.ch/R-manual/R-devel/library/base/html/Rhome.html. 

3. Enable automatic reference re-resolution in the editor. For that, you need to enable the corresponding flag ("Automatically run reference resolve quick fixes")
   on the Editor page in the Project settings (menu File&gt;Settings...&gt;Editor&gt; General) as shown: 
   
   ![QuickRef](../images/EnableQuickRefResolution.png){:height="90%" width="90%"}
