![MetaR logo](../images/MetaR-logo-4-SMALL-300x111.png)

## Installation instructions for MacOS users

System requirements
-
[MetaR](https://github.com/MetaR-Languages/MetaR) can be installed only if these requirements are met:
* MacOS Sierra 10.12+
* 4 GB RAM minimum, 8 GB RAM recommended
* 4 GB hard disk space, SSD recommended
* 1024x768 minimum screen resolution

Install software required by MetaR
-
1. Download and install Jetbrains MPS 2019.1.5 bundled with Java 8 (205 MB) from [https://download-cf.jetbrains.com/mps/2019.1/MPS-2019.1.5-macos-jdk-bundled.dmg](https://download-cf.jetbrains.com/mps/2019.1/MPS-2019.1.5-macos-jdk-bundled.dmg)

2. Install Docker Community Edition from [https://store.docker.com/search?type=edition&offering=community](https://store.docker.com/search?type=edition&offering=community) (you need to register for the download). 

    Depending on your machine’s system, follow the simple steps described on the download page to activate Docker on your system. Then, from the Terminal application, type the following command:

        docker pull artifacts/metar:latest

    then press enter/return. This will download a docker image we will use to execute MetaR analyses.
   
Install MetaR
-    
1. Install the MPS metaR plugin
    
    1.1 Start the MPS application and open-up the plugin manager in MPS (menu MPS > Preferences… > Plugins)
    
    1.2 Click on the top-right gear image and then select “Manage Plugin Repositories…” from the menu.
    
    ![Repo](../images/AddRepo2019.1.png){:height="30%" width="30%"}

    1.3 In the new window, click on the “+” button and add the following URL: http://mpsrepo.slisson.de/
  
    ![Repo](../images/AddRepoURL2019.1.png){:height="50%" width="50%"}
    
2. Back on the “Plugins” window, click on "Marketplace" and search for "MetaR" and click on the install button of the plugin _org.campagnelab.MetaR_. Restart the application to activate the plugin.
  
    ![PluginInstall](../images/InstallMetaR2019.1.png){:height="30%" width="60%"}
    
3. After restarting, open MPS, go back in the plugin manager (menu MPS > Preferences… > Plugins), select the "Installed" tab, and make sure the MetaR plugin is not listed red.     
   
    ![PluginCheck](../images/CheckMetaR2019.1.png){:height="50%" width="50%"}
    
Configuration
-    

1. Define the following Path Variable (menu MPS&gt;Preferences...&gt;Appearance &amp; Behavior&gt;Path Variables):
    * **Name**: _org.campagnelab.metaR.results_dir_
    * **Value**: an arbitrary folder <strong>under /Users in Mac OS X </strong>where you want the results of MetaR analyses to be placed. (Avoid a path with spaces.)
  
    ![AddVariable](../images/AddVariable.png){:height="80%" width="80%"}

2. Enable automatic reference re-resolution in the editor. For that, you need to enable the corresponding flag ("Automatically run reference resolve quick fixes")
   on the Editor page in the Project settings (menu MPS&gt;Preferences...&gt;Editor&gt; General) as shown: 
   
   ![QuickRef](../images/EnableQuickRefResolution.png){:height="90%" width="90%"}
