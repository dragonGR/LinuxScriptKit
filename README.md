# LinuxScriptKit

"LinuxScriptKit" is a collection of scripts that i use to simplify the setup and management of a Linux system. This repository includes a variety of scripts, from system maintenance to productivity tools, that can be used to streamline your workflow and optimize your Linux environment.

## How to use

When it comes to running a bash script, there are multiple ways to do it. One way is to use the "./" command followed by the name of the script file. This tells the shell to execute the script as an executable file. Another way is to use the "bash" command followed by the name of the script file. This tells the shell to run the script using the Bash interpreter. Similarly, you can also use the "sh" command followed by the name of the script file to execute the script using the shell interpreter. It's worth noting that these methods may differ depending on the system and the shell being used.

## NodeAndNpmInstaller

This script installs NVM and uses Node.js version 16.13.1. It first checks if Node.js and npm are installed, and uninstalls them if they are. Then it proceeds with installing NVM, which is a version manager for Node.js, and loads it into the current shell session. After that, it installs Node.js version 16.13.1, sets it as the default version, and displays the version in use.

We have decided to use Node.js version 16.13.1 because it is known to be working with every project we have, and the Node.js community also agrees that it is the most stable version with very few bugs. We have found that the latest Node.js versions are mostly broken and require most of the packages to be updated to today's standards. By using a stable version, we can ensure that our projects are working as expected and avoid any issues that may arise from using a bleeding-edge version of Node.js. Overall, this script helps us maintain consistency across our projects and ensures that we are using a reliable and stable version of Node.js.

## MongoInstaller

This script is a cross-platform installation script for MongoDB and MongoDB Compass. It is designed to work on both Debian and Arch based systems and automates the installation process, making it simple and efficient for users. The script first checks the system type (Debian or Arch) and then installs the appropriate packages using the respective package managers (APT or Pacman).

For Debian based systems, the script adds the MongoDB repository to APT sources and imports the MongoDB public GPG key to ensure secure installation. It then installs the MongoDB server and MongoDB Compass using the apt-get command. On the other hand, for Arch based systems, the script uses pacman to install MongoDB and yay to install MongoDB Compass. Overall, the script makes it easy to install MongoDB and MongoDB Compass on either Debian or Arch based systems, saving users time and effort in the installation process.

## JavaInstaller

For both Debian and Arch based systems, the script adds the MongoDB repository to the APT sources using the apt-key and apt-add-repository commands. The MongoDB package is then installed using the apt-get or pacman command, depending on the system. The mongodb-org package includes the MongoDB server, client, and other tools, while the mongodb-compass package includes the MongoDB Compass GUI tool.

After the packages are installed, the script checks if the installation was successful. If MongoDB Compass is installed successfully, the script removes the downloaded MongoDB Compass file using the rm command. Finally, the script prints a message indicating that the installation was successful.
