## Command Line Setup Steps for macOS

Launch **`Terminal`** in macOS, located at **`/Applications/Utilities/Terminal.app`**

> If your current account doesn't have admin privileges, switch users by entering the following command (substituting the username of the admin account). Press return and enter your password at the prompt.
>
>    `su your_admin_name`
>
> If you don't remember your admin username, the following command will list the users on your system.
>
>    `ls /Users/`

To install a bundle of command-line tools provided by Apple, paste the following line into the terminal window and press return. When prompted, click "Install," then "Agree."

    xcode-select --install

Run the following command to install the **`Homebrew`** package manager. Enter your password at the prompt to proceed.

    /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

Next, enter this command to update Homebrew.

    brew update

> If Homebrew returns an error, enter the following command to give it the permissions it expects.
>
>    `sudo chown $(whoami):admin /usr/local && sudo chown -R $(whoami):admin /usr/local`

Now you can install command-line programs in a single line, like so:

```
brew install wget

brew install youtube-dl
```

Python is installed by default in macOS, but we’ll want to install a fresh copy through Homebrew. This version includes the **`pip`** package manager and a few other tools Apple left out.

```
brew install python

brew link --overwrite python
```

Before we go further, we should update pip. The **`-U`** option tells pip to update a package's dependencies to their most recent versions.

```
pip install -U pip
```

Enter the following command to install several useful Python packages.

```
pip install -U jupyter numpy scipy matplotlib pandas
```
