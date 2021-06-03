Dockerize Great Number Game using MySQL DB
1. Download or pull this repository.
2. After downloading, your pc/laptop should have Docker and MySQL Workbench on it.
3. Make sure you extract/copy this repository in Ubuntu's /home/[yourname] directory. To locate Ubuntu's directory, click Start then type \\wsl$ and hit enter. A new windows explorer should pop up and will contain 3 folders. Just double click on the Ubuntu folder. From there you will see a home folder, and in the home folder, you will see your name. This is where you should paste/extract this repository. Paste/Extract it in /home/[yourname] directory. Example: /home/prinsipeces/dockerize_express
4. Instead of opening VS Code directly from your Desktop, open VS Code using a command prompt.
    - Open a command prompt and type in wsl and press enter. Your command prompt will switch from a windows cli, to a linux terminal
    - You will then be able to cd in to /home/[yourname] directory. Example: cd /home/prinsipeces/dockerize_express
    - Then type in code . and press enter. The (dot) symbol is included.
    - VS Code will open, but instead of a Windows VS Code, it will open a VS Code from Ubuntu. You will also need to install the Docker extension for this VS Code.
    - Finally, to build and run your container, just right click on docker-compose.yml and click Compose Up. Just wait for the installation and downloading of dependencies and files.
5. While waiting for the installation/downloading to finish, open your MySQL Workbench and create a new connection.
    - Give/Enter any connection name.
    - Hostname should be on localhost/127.0.0.1
    - On this repository I use port 3307. You can see and change it, just open the .yml file and you can see the port settings under the db services.
    - Username is root
    - Password is password
    - Deafult schema is hh
    - Click the test connect to test if it's connected or not.
    - Finally, just click the new connection you created and it will automatically load the tables and datas.
6. Switch to your VS Code and go to the docker extension, you will see all the connected containers in the containers tab. If it has a play button on it, it just means that it is already connected.
7. If all connections are ready, then go to your browser and type on the url localhost:3001, where 3001 is the port connection outside the docker. You can also see or change it on the .yml file under the web_app services.
8. Now, go on and play the great number game. You can also check the results changing on the sessions table on the database.