## About the course

This repository is for use with the Pearson Publishing live webinar
"Machine Learning with `PyTorch`."  Versions of this material are
used by other training provided by David Mertz and [KDM
Training](http://kdm.training).

If you have attended one of the webinars using this material, I
encourage you to complete the survey on it at: [Machine Learning
Webinar survey](https://goo.gl/pghpzD).  As folks fill this out, we
will fold back the updated answers into the dataset used in the
lessons themselves.

## Installing training materials

Before attending this course, please configure the environments you
will need.  Within the repository, find the file `requirements.txt`
to install software using `pip`, or the file `environment.yml` to
install software using `conda`.  I.e.:

```bash
$ conda env create -f environment.yml
$ conda activate Pearson-PyTorch
(Pearson-ML) $ jupyter notebook Outline.ipynb
```

Or

```bash
$ pip install -r requirements.txt
$ juypter notebook Outline.ipynb
```

PyTorch often works vastly faster when utilizing a CUDA GPU to
perform training.  Students who wish to be able to follow along
running the material on their own machines in real time, are advised
to obtain access to a GPU machine while attending this webinar.
 
Numerous cloud services provide access to rented GPU instances are
reasonable hourly costs.  AWS EC2 instances are very well known, and
can be leased with good GPU configurations.  The author is very fond
of a service called vast.ai (https://vast.ai/) that he will use
during presentation of the webinar.   Of course, if you have any
moderately recent CUDA-enabled GPU on your home or work machine, you
will be fine also.

If you run this material on a leased cloud GPU, you will probably
start with a fairly minimal base Docker image.  It will probably be
a good idea to install a few tools using the system installer (some
of those are used in the lessons themselves, but nothing important
depends on them if you follow without those available).

I setup a new cloud instance with these steps, once I open a
terminal into that machine:

```bash
$ git clone https://github.com/DavidMertz/PyTorch-webinar.git
$ cd PyTorch-webinar/
$ apt-get update  # Make sure latest repo information
$ apt-get install jq curl tree vim -y
$ pip install --upgrade pip  # latest version changes often
$  pip install -r requirements.txt
```

## Recommended reading

* [(Video) Machine Learning with PyTorch](https://learning.oreilly.com/videos/machine-learning-with/9780135627105), by David Mertz.

* [(Video) Machine Learning with scikit-learn LiveLessons](https://www.oreilly.com/library/view/machine-learning-with/9780135474198/), by David Mertz.

* [Documentation of PyTorch](https://pytorch.org/docs/stable/index.html)

* [Beginner Machine Learning with `scikit-learn`](https://github.com/DavidMertz/ML-Live-Beginner).

* [Intermediate Machine Learning with `scikit-learn`](https://github.com/DavidMertz/ML-Live-Intermediate).

* _Hands-On Machine Learning with Scikit-Learn and TensorFlow: Concepts, Tools, and Techniques to Build Intelligent Systems_, by Aurélien Géron.

* _Deep Learning with Python_, by Francois Chollet.

* _Introduction to Machine Learning with Python: A Guide for Data Scientists_, by by Andreas C. Müller & Sarah Guido.

* _Python Data Science Handbook: Essential Tools for Working with Data_, by Jake VanderPlas.

* _Data Science from Scratch: First Principles with Python_, by Joel Grus.

