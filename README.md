# Sikuil_RPI4


Update and Upgrade Your System: Ensure your system is up to date:

sh
Copy code
sudo apt update
sudo apt upgrade
Install Java: Sikuli requires Java to run. Install Java with:

sh
Copy code
sudo apt install openjdk-11-jdk
Check the Java installation:

sh
Copy code
java -version
Install Dependencies: Install necessary dependencies, including the tools Sikuli needs to interact with the GUI:

sh
Copy code
sudo apt install wmctrl xdotool
Download Sikuli: Navigate to the SikuliX download page on another machine, as you might find it challenging to navigate and download directly on the RPI4's browser depending on your setup. Download the latest SikuliX version that is compatible with Linux.

Transfer Sikuli to RPI4: If you downloaded Sikuli on another machine, transfer it to your RPI4. You can use scp or a USB drive to transfer the file.

Install Sikuli: Once the SikuliX jar file is on your RPI4, you can run it with Java. Navigate to the directory where you placed the SikuliX jar file and run:

sh
Copy code
java -jar sikulix.jar
This command should launch the SikuliX IDE setup process. Follow the on-screen instructions to complete the installation.

Verify Installation: After installing, try running SikuliX again to ensure it opens correctly.

sh
Copy code
java -jar sikulix.jar
Running Your Sikuli Scripts: Now, you can create and run Sikuli scripts using the SikuliX IDE.

Remember, Sikuli is heavily dependent on screen resolution and the graphical interface, so running it on a headless RPI4 (without a connected monitor) won't work out of the box. Also, performance might vary due to the RPI4's hardware constraints compared to a typical desktop environment where Sikuli is usually run.



 ^Cadmin@raspberrypi:~/SikuliX $ java -jar sikulixide-2.0.5-lux.jar 
[error] RunTime:loadLib: libJXGrabKey.so (failed) probably dependent libs missing:
/home/admin/.Sikulix/SikulixLibs/libJXGrabKey.so: /home/admin/.Sikulix/SikulixLibs/libJXGrabKey.so: cannot open shared object file: No such file or directory (Possible cause: can't load AMD 64 .so on a AARCH64 platform)
[error] Save your work, correct the problem and restart the IDE!
[error] see: https://github.com/RaiMan/SikuliX1/wiki/macOS-Linux:-Support-Libraries-for-OpenCV-4
TERMINATING: problem with native library: libJXGrabKey.so
Opening in existing browser session.
