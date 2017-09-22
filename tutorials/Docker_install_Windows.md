## Installing Docker for Windows 10

<!--
https://docs.docker.com/docker-for-windows/install/
Docker for Windows installation guide
-->

Download [Docker Community Edition for Windows](https://store.docker.com/search?type=edition&offering=community).
*Docker does work with Windows 10 Home Edition, because it does not come with Hyper-V (Microsoft's virtual machine). You will need education edition or higher for it to install properly. The alternative is to download Docker Toolbox which installs an Oracle virtual machine (VMBox). However, there may be conflicts if there are existing virtual machines installed. 

Double click the Docker installer file when it's finished downloading.

When the installation process is complete, a file called `Docker for Windows` will appear on the desktop. Double click it.

An alert window will appear at the bottom right corner of your screen asking you to log out of your Windows user account and log back in. Do so.

When you've logged back in, double click `Docker for Windows` on your desktop.

An alert window will appear asking you to enable Hyper-V. Click "OK." After a moment your computer will restart.

Double click `Docker for Windows` on your desktop. After a minute or so, an alert window will appear at the bottom right of your screen telling you Docker is ready.

Next, click the `^` icon in the Windows toolbar, at the bottom right of the screen. In the menu that pops up, right click the Docker icon (a whale with small boxes on its back). Click "Settings."

Click "Shared Drives" in the left column, then click the check box next to "C." Click "Apply" to confirm, then enter your user password at the prompt.

Docker is now installed and ready to go. Open the `Windows PowerShell` application and enter the following command to download the Docker image for this class.


```
docker pull pcda17/ubuntu-container
```

To launch the Docker container, paste the following command into PowerShell and press return (using your Windows username instead of `**your-username**`).

```
docker run --name pcda_ubuntu -ti -p 8889:8889 --volume C:\Users\**your-username**\Desktop\sharedfolder\:/sharedfolder/ pcda17/ubuntu-container bash
```

*Note: If you aren't able to paste text into PowerShell, right click the bar at the top of the PowerShell window, then select `Edit > Paste`*.
