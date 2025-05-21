**FTP Client**

**What the program does:**

This is an FTP Client that sends commands to an FTP server. The FTP server used for testing is ftp://ftp.3700.network.  
FTP is a client-server oriented protocol for uploading, downloading, and managing files. An FTP server will listen for incoming connections from clients and then execute their requests. 

**Description:**

This Python script provides an FTP client implementation for interacting with FTP servers. It supports basic FTP operations such as connecting to a server, logging in, listing directories, making/removing directories, uploading/downloading files, and deleting files.

**Functions/Features:**

Connect to an FTP server using TCP sockets.  
Login to the FTP server with username and password.  
Enter passive mode for data transfer.  
List the contents of a remote directory.  
Make a remote directory.  
Remove a remote directory.  
Upload a file to the server.  
Download a file from the server.  
Delete a file on the server.  
Move a file to and from the server.

**Prerequisites:**

Python 3.x  
Access to FTP server  
Permission to access FTP servers

**How to use:**

Download the script 3700ftp.py.  
Open a terminal or command prompt.  
Navigate to the directory containing the script.  
Run the script with appropriate command-line arguments.

Command-line Arguments  
ls <FTP_URL>: List the contents of the specified directory on the FTP server.  
rm <FTP_URL>: Delete a file on the FTP server.  
rmdir <FTP_URL>: Remove a directory on the FTP server.  
mkdir <FTP_URL>: Make a directory on the FTP server.  
cp <LOCAL_FILE_PATH> <FTP_URL>: Copy a file from the local machine to the FTP server.  
cp <FTP_URL> <LOCAL_FILE_PATH>: Copy a file from the FTP server to the local machine  
cp <LOCAL_FILE_PATH> <FTP_URL>: Move a file from the local machine to the FTP server.  
cp <FTP_URL> <LOCAL_FILE_PATH>: Move a file from the FTP server to the local machine

**Example Usage:**

./3700ftp ls ftp://adarshj:<password>@ftp.3700.network  
./3700ftp mkdir ftp://adarshj:<password>@ftp.3700.network/test  
./3700ftp cp hw3.txt ftp://adarshj:f1aeda0b54830fdf0f3063b12b96f1649b079305ab63aeb44b3e39ac12efa3a5@ftp.3700.network/hw4.txt  
./3700ftp cp ftp://adarshj:f1aeda0b54830fdf0f3063b12b96f1649b079305ab63aeb44b3e39ac12efa3a5@ftp.3700.network/hw3.txt hw4.txt

**Remember to replace username, password, and the ftp server with your own data.**

Author  
Adarsh Jayaram
