##Week 7: Data and Politics / CSVs and APIs


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


Right click the following links and save the following Jupyter notebook files to `sharedfolder` on your desktop. Navigate to [localhost:8889](localhost:8889) in your browser to open each notebook.

1. [https://raw.githubusercontent.com/pcda17/pcda17.github.io/master/week-07.1_CSV-Input-Output.ipynb](CSV Input/Output)

2. [https://github.com/pcda17/pcda17.github.io/blob/master/week-07.2_Google_Books_API.ipynb](Google Books API)

3. [https://raw.githubusercontent.com/pcda17/pcda17.github.io/master/Week-06_Scraping-and-Parsing-XML.ipynb](Scraping and Parsing XML Finding Aids)



