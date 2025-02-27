---
uid: Installing_the_DataMiner_Cube_desktop_application
---

# Installing the DataMiner Cube desktop application

There are several ways to install the DataMiner Cube desktop application, depending on your DataMiner version.

## From DataMiner 10.0.0/10.0.4 onwards

1. Browse to your DMA using a different browser than Internet Explorer.

1. Enter your username and password to log in.

1. Install DataMiner Cube in one of the following ways:

   - **Prior to DataMiner 10.0.9**: To install DataMiner Cube using the ClickOnce web installer, on the landing page, click the button *Install DataMiner Cube* and select *Click-once installation*.

   - **From DataMiner 10.0.9 onwards**:

     1. On the DataMiner landing page, select *Desktop installation* and run the downloaded file.

     1. In the installation window, open the *Options* section and adjust the options depending on whether you want a shortcut to be added to the desktop and/or start menu and on whether you want DataMiner Cube to start with Windows.

     1. Click *Install*.

     > [!NOTE]
     > - Once the desktop app has been installed, it will be updated automatically when you connect to other DataMiner versions.
     > - To install the app, you need Modify access to the folders `%AppData%\Skyline` and `%LocalAppData%\Skyline`, as well as write access to the key `HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall`.
     > - To be able to run the app, you need Execute access for the files `%LocalAppData%\Skyline\DataMiner\DataMinerCube\DataMinerCube.exe` and `%LocalAppData%\Skyline\DataMiner\DataMinerCube\CefSharp\version\architecture\CefSharp.BrowserSubprocess.exe`.
     > - To create a desktop shortcut, you need Modify access to the folder `%UserProfile%\Desktop`.
     > - To create a start menu shortcut, you need Modify access to the folder `%AppData%\Microsoft\Windows\Start Menu\Programs`.
     > - The *Start with Windows* feature requires write access to the key `HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Run`.
     > - The eventing communication mode will only be available if the firewall allows the application `*%LocalAppData%\Skyline\DataMiner\DataMinerCube\DataMinerCube.exe` to accept incoming connections.

   - From DataMiner 10.2.0/10.2.2 onwards, it is also possible to install DataMiner Cube using an **MSI installer**, but this is **not recommended as this requires manual updating** when a new version is available. Typically, this is only used by a system administrator to deploy DataMiner Cube in bulk on many client machines at the same time using some form of automation. The MSI installer can be found in the folder `C:\Skyline DataMiner\Webpages\Tools\Installs` on each DMA.

     > [!NOTE]
     > - If you install DataMiner Cube with the MSI installer, you will also have to manually install the corresponding CefSharp version using the separate CefSharp MSI installation package, which is available on demand.
     > - Prior to DataMiner 10.0.9, the MSI installer is available via the DataMiner landing page, via *Install DataMiner Cube* > *Other install options* > *MSI installer*.

## From DataMiner 10.0.2 onwards

If you browse to your DMA using a browser that does not support DataMiner Cube, depending on your configuration, a landing page will be displayed.

On the landing page, click the user icon in the top-right corner and select the DataMiner Cube installation option you prefer under *Standalone applications*.

## Prior to DataMiner 10.0.0/10.0.2

On the landing page, click *Install DataMiner Cube*.

Alternatively, go to `http://[DMA name]/DataminerCubeStandalone/publish.htm` and click *Install*.

> [!TIP]
> See also: [Configuring the default landing page](xref:DMA_configuration_related_to_client_applications#configuring-the-default-landing-page)

> [!NOTE]
> Once you have installed the application, it will automatically be updated whenever a new version is available.
