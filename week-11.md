## Week 11


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

Download a Jupyter notebook from the list below to `sharedfolder` on your desktop.


Navigate to [localhost:8889](localhost:8889) in your browser to open the notebook.


### Jupyter Notebooks

- [Reference Snippets: Strings and Lists](https://github.com/pcda17/pcda17.github.io/blob/master/Reference_Snippets_--_Strings_and_Lists.ipynb)

- [Unsupervised Learning: k-means clustering](https://github.com/pcda17/pcda17.github.io/blob/master/Week-11.1_Clustering.ipynb)

- [Supervised Learning](https://github.com/pcda17/pcda17.github.io/blob/master/Week-11.2_Supervised-learning.ipynb)

- [New York Times Article Scraper](https://github.com/pcda17/pcda17.github.io/blob/master/Week-11_NYT_Article_Scrape.ipynb)

### Resources

- [scikit-learn cheat sheet](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Scikit_Learn_Cheat_Sheet_Python.pdf)

- [scikit-learn: Clustering Overview](http://scikit-learn.org/stable/modules/clustering.html)

- [scikit-learn: Supervised Learning Overview](http://scikit-learn.org/stable/tutorial/statistical_inference/supervised_learning.html)

