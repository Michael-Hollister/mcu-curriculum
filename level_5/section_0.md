## Setup - SWRI

### Downloads

* Download IntelliJ from their site: [JetBrains IntelliJ IDEA Community Edition](http://www.jetbrains.com/idea/). Click on the `Download` button at the top of the page to take you to the downloads section. You will want to download the Community edition, which is a free version of JetBrains commercial IDE, and it has lots of the same features.

* We'll also need to download [Forge](http://files.minecraftforge.net/maven/net/minecraftforge/forge/1.11.2-13.20.1.2429/forge-1.11.2-13.20.1.2429-mdk.zip), which is a modding API.

* Also download the [Java SDK 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html). You will have to click the `Accept License Agreement` button to download the sofware. Download the correct version for your system from that page.

* If you are using Windows, also download [7-Zip](http://www.7-zip.org). We will need this program for creating textures later on.

### Installation

1. Install the Java SDK and 7-Zip by running the files you downloaded.

2. Run the IntelliJ installer, and follow its instructions. Make sure you have installed the Java SDK before installing IntelliJ, it will make the setup process easier.

3. Make a new folder on the desktop and name it `Minecraft Dev` and drag the `forge` folder into it. The forge folder is a .zip file so we need to extract it. Put the extracted folder into the Minecraft Dev folder as well.

### Getting started for Windows

1. Hold shift and right click inside the folder `forge-1.11.2-13.20.0.2228-mdk`. Click on `Open command window here`. Then type `gradlew setupDecompWorkspace --refresh-dependencies` and press `Enter`. This will download the Minecraft source code and decompile it so we can work with it to make our mod.

2. Once you get `BUILD SUCCESSFUL` type `gradlew idea` and press `Enter`.

### Troubleshooting:

The most common error is the build failing with a message saying "JAVA_HOME does not point to JDK":

1. Click start  
2. Right-click Computer  (for Windows 8 open up file explorer and right-click "This PC")  
3. Click properties  
4. On the left side click advanced system settings  
5. At the bottom of the pop-up, click Environment Variables  
6. Under system variables (second section of pop-up) click new  
7. Name it JAVA_HOME  
8. The value should point to your JDK 8 folder (something like "C:\Program Files\Java\jdk1.8.0_131")  
9. Click ok  
10. Close and re-open command prompt and run the command again.  

