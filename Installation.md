# Installing Docker Desktop on Windows
The following tasks must be completed to install Docker Desktop:

## Step 1: Download and Install Docker Desktop on Windows through GUI
1. Download [Docker Desktop](https://desktop.docker.com/win/main/amd64/Docker%20Desktop%20Installer.exe) for Windows installer.
2. Double-click the installer package to run the installer.
3. On the **Configuration** page, select **Enable WSL 2 Windows Feature** and then click **OK**. The installation component and its dependencies gets automatically installed.
4. After installation, click the **Close and Log out** button. The installer application is closed and the current user is logged out.
> **Note**: After installation, you may choose to restart the system.

## Step 2: Check Docker Version and Open the Docker Desktop Application
1. Open **Powershell** on your system
2. Type or copy/paste the following command:
    ```
    docker --version
    ```
    The result displays the version of the docker. <br/>
    
    > **Note**: In case the installation fails or docker is not completely installed, an error message, "The term 'docker' is not recognized" is displayed.
 3. Press the Windows key and type, "Docker Desktop" in the search field
 4. Open the application. The landing page
 5. 
## Step 3: Run Sample Containerized Image of an Application using Docker
