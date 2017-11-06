##Week 9: Your Culture, Your Data



Open Terminal in macOS and launch our Docker container:

```
docker rm -f pcda_ubuntu
docker pull pcda17/ubuntu-container
docker run --name pcda_ubuntu -ti -p 8889:8889 --volume ~/Desktop/sharedfolder/:/sharedfolder/ pcda17/ubuntu-container
```

In Windows 10, open PowerShell and enter the following to launch the Docker container:

```
docker rm -f pcda_ubuntu
docker pull pcda17/ubuntu-container
docker run --name pcda_ubuntu -ti -p 8889:8889 --volume C:\Users\***username_here***\Desktop\sharedfolder:/sharedfolder/ pcda17/ubuntu-container
```

Right click the following link and save the Jupyter notebook file to `sharedfolder` on your desktop.


- [Data Visualization and Statistics](https://raw.githubusercontent.com/pcda17/pcda17.github.io/master/Week-09_Machine-Learning.ipynb)


Navigate to [localhost:8889](localhost:8889) in your browser to open the notebook.
