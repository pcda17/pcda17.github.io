
<!--
### Launch Jupyter notebook using Docker

Enter the following command to run the Jupyter notebook Docker container.

```
docker rm -f pcda_notebook

docker run -it --name pcda_notebook -p 8888:8888 -v ~/Desktop/sharedfolder/:/sharedfolder/ jupyter/minimal-notebook
```

In your terminal window, you should see a message similar to the following.

>Copy/paste this URL into your browser when you connect for the first time, to login with a token:
>    http://localhost:8888/?token=e00d450b9e9f2518b5d36bb814cd56dbc2fb67d1a8af8df0







### Pre-installed software on Computer lab machines

- Apple command line tools
- Atom (text editor)
- VLC Media Player
- Homebrew (package manager)
- Python 2.7
- pip (package manager for Python)
- Jupyter (code editor)
- ExifTool (command-line metadata reader)
- FFmpeg (command-line media encoder)
- youtube-dl (command-line video downloader)
- Wget (command-line file downloader)

#### **2.** Installing Command Line Tools and Homebrew (laptops only) <!-- We may not need this part since students won't be installing on their own computers. We can add in a "if you want to go further than the class" kind of page but we can't get into troubleshooting their installations all semester-->

First we’ll install the package manager [Homebrew](#), which will expedite the process of installing other command-line programs. Open a window in Terminal, then paste the following line and press return.

    /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

> _Tip:_ If you aren’t currently running as an administrator, you’ll need to switch to an admin account first, then re-enter the line above. Enter `su` followed by the name of an admin account, then enter the account’s password at the prompt.
>
>     su adminname

The following window will appear. Click “Install” to download a set of standard tools for Unix-like operating systems. Alternately, you can get the same tools by installing Apple’s **Xcode** development environment from the [App Store](#) (~4GB).

![](week/1/week/1/Image-0.png)

A license agreement window will appear. Read (or at least skim) the text, then click “Agree.” The software will take a minute or two to download and install.

![](week/1/Image-1.png)

While we wait, let’s talk a bit about the command-line interface.



#### **4.**Installing Homebrew and Python

When Apple’s command-line tools are ready, a window will pop up that says “The software was installed.” Click “Done.”


Switch back to your original terminal window and press return to continue installing Homebrew. Enter your password at the prompt. Homebrew will take a minute or two to download and install. When it’s finished, your terminal window should look something like this.

![](week/1/Image-4.png)

Let’s make sure Homebrew is up to date. This shouldn’t take more than a minute.

    brew update

A version of Python comes pre-installed with OS X, but to make our lives easier we’ll install a fresh copy using Homebrew that includes the pip package manager and a few other tools Apple left out. We’ll be using Python 2.7, by the way. This will take 5 or 10 minutes to download and install.

    brew install -U python

> **Tip:** If the command above returns “Error: Cannot write to /usr/local/Cellar,” this is due to a permissions tweak in a recent version of OS X. Enter the following commands one at a time to fix the issue, entering your password after the last line.

>     chgrp -R admin /usr/local
>     chmod -R g+w /usr/local
>     chgrp -R admin /Library/Caches/Homebrew
>     sudo chmod -R g+w /Library/Caches/Homebrew






-->






#### **1.** Student and instructor introductions

### Pre-installed software on Computer lab machines

- Apple command line tools
- TextWrangler (text editor)
- VLC Media Player
- Homebrew (package manager)
- Python 2.7
- pip (package manager for Python)
- Jupyter (code editor)
- ExifTool (command-line metadata reader)
- FFmpeg (command-line media encoder)
- youtube-dl (command-line video downloader)
- Wget (command-line file downloader)

#### **2.** Installing Command Line Tools and Homebrew (laptops only) <!-- We may not need this part since students won't be installing on their own computers. We can add in a "if you want to go further than the class" kind of page but we can't get into troubleshooting their installations all semester-->

First we’ll install the package manager [Homebrew](#), which will expedite the process of installing other command-line programs. Open a window in Terminal, then paste the following line and press return.

    /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

> _Tip:_ If you aren’t currently running as an administrator, you’ll need to switch to an admin account first, then re-enter the line above. Enter `su` followed by the name of an admin account, then enter the account’s password at the prompt.
>
>     su adminname

The following window will appear. Click “Install” to download a set of standard tools for Unix-like operating systems. Alternately, you can get the same tools by installing Apple’s **Xcode** development environment from the [App Store](#) (~4GB).

![](week/1/week/1/Image-0.png)

A license agreement window will appear. Read (or at least skim) the text, then click “Agree.” The software will take a minute or two to download and install.

![](week/1/Image-1.png)

#### **4.**Installing Homebrew and Python

When Apple’s command-line tools are ready, a window will pop up that says “The software was installed.” Click “Done.”


Switch back to your original terminal window and press return to continue installing Homebrew. Enter your password at the prompt. Homebrew will take a minute or two to download and install. When it’s finished, your terminal window should look something like this.

![](week/1/Image-4.png)

Let’s make sure Homebrew is up to date. This shouldn’t take more than a minute.

    brew update

A version of Python comes pre-installed with OS X, but to make our lives easier we’ll install a fresh copy using Homebrew that includes the pip package manager and a few other tools Apple left out. We’ll be using Python 2.7, by the way. This will take 5 or 10 minutes to download and install.

    brew install -U python

> **Tip:** If the command above returns “Error: Cannot write to /usr/local/Cellar,” this is due to a permissions tweak in a recent version of OS X. Enter the following commands one at a time to fix the issue, entering your password after the last line.

>     chgrp -R admin /usr/local
>     chmod -R g+w /usr/local
>     chgrp -R admin /Library/Caches/Homebrew
>     sudo chmod -R g+w /Library/Caches/Homebrew

#### **8.** Installing software with Homebrew and pip

Now that Python is installed, enter the following lines one at a time at the terminal to view Python’s location in the file system and its version number.

    which python
    python --version

Homebrew has automatically installed **pip**, a package manager for software libraries we can access within Python. Let’s update our copy of pip to the latest version (laptop users only).

    pip install --upgrade pip

> _Note:_ When we include the `--upgrade` option, pip will download the newest versions of any dependencies associated with the software we’re installing. The abbreviated form of this option is `-U`.

 Next, install **[Jupyter](#)** using pip.

    pip install -U jupyter

Install **[ExifTool](#)**, a metadata viewer and editor for a wide range of media formats (laptop users only).

    brew install exiftool

Finally, install **[Wget](#)**, a command-line tool for downloading Web data (laptop users only).

    brew install wget

#### Download a Web page from the shell
Begin by `cd`ing to Desktop.

    cd /sharedfolder

Then enter `wget` followed by any URL.

    wget http://google.com

![](week/1/Image-9.png)

If you’re connected to the Internet and Wget is installed correctly, you should see feedback in the shell that looks something like the above. In this case, Wget has saved Google’s “index.html” file to the desktop. Either view the file in the shell using `less` or open it in TextWrangler.

![](week/1/Image-10.png)

To make the file more readable in TextWrangler, go to the toolbar and select `View > Text Display > Soft Wrap Text`.

Wget is an amazingly versatile tool, and we’ll return to it in later weeks. In the meantime, the manual is worth a skim.

    man wget
