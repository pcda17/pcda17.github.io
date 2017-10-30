## Week 8: Statistics and Visualization



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


- [Data Visualization and Statistics](https://raw.githubusercontent.com/pcda17/pcda17.github.io/master/week-8_Stats-and-Visualization.ipynb)


Navigate to [localhost:8889](localhost:8889) in your browser to open the notebook.


### Resources


- [Matplotlib gallery](https://matplotlib.org/gallery.html)

- [Matplotlib tutorial](http://www.labri.fr/perso/nrougier/teaching/matplotlib/)

- [Numpy quickstart tutorial](https://docs.scipy.org/doc/numpy-dev/user/quickstart.html)

- [scipy.stats tutorial](https://docs.scipy.org/doc/scipy/reference/tutorial/stats.html)

- [An introduction to Numpy and SciPy](https://engineering.ucsb.edu/~shell/che210d/numpy.pdf)

<!--
## Topics to Cover

- Descriptive statistics using numpy Python module
- Creating graphs in the matplotlib Python module

- Visualization

    - Tutorial source: [http://www.labri.fr/perso/nrougier/teaching/matplotlib/](http://www.labri.fr/perso/nrougier/teaching/matplotlib/)


Tutorial source for statistical tests on literary works:

- http://digitalhumanities.org/companion/view?docId=blackwell/9781405103213/9781405103213.xml&doc.view=print&chunk.id=ss1-4-4&toc.depth=1&toc.id=0

-->
