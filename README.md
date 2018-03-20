# Data Science Resources
This is an opinionated list of useful resources for data science. Feel free to
contribute.
___
## Contents
- [Beginner Zone](#beginner-zone)
- [General Computing](#general-computing)
  - [Command Line](#command-line)
  - [Text Editors](#text-editors)
  - [Markup Languages](#markup-languages)
- [Programming Languages](#programming-languages)
  - [Python](#python)
  - [R](#r)
  - [Other](#other)
- [Databases](#databases)
- [Data Visualization](#data-visualization)
  - [Data Visulaization Software](#data-visualization-software)
  - [Data Visualization Books and Links](#data-visualization-books-and-links)
- [Math](#math)
  - [Calculus](#calculus)
  - [Linear Algebra](#linear-algebra)
  - [Optimization](#optimization)
  - [Probability](#probability)
- [Statistics](#statistics)
  - [Core Concepts](#core-concepts)
  - [Bayesian Statistics](#bayesian-statistics)
  - [Time Series](#time-series)
  - [Statistical Software](#statistical-software)
- [Machine Learning](#machine-learning)
  - [Basics](#basics)
  - [Neural Networks and Deep Learning](#neural-networks-and-deep-learning)
- [Other Resources](#other-resources)
  - [Blogs](#blogs)
  - [News](#news)
  - [Podcasts](#podcasts)

## Beginner Zone
___
**Q:** What is data science?<br>
**A:** Statistics in the 21st century.

**Q:** What is machine learning?<br>
**A:** Statisics as practiced by computer scientists.

**Q:** Where do I get started?<br>
**A:** Learn to use the [command line](#command-line), then learn [R](#r) if
you're a statistician or [Python](#python) if you're anyone else. From there,
learn some math.

**Q:** Do I need to know all of this stuff to be a data scientist?<br>
**A:** No. Don't even try it.

**Q:** I don't like math. Can I still be a data scientist?<br>
**A:** The core math topics are pretty important, but you can choose to
focus more on the data management side, perhaps along with some
visualization tools. Don't expect to do much machine learning, though.

**Q:** I don't like computers. Can I still be a data scientist?<br>
**A:** Not unless you *really* like math.
___
## General Computing
- [Draw.io](https://www.draw.io/) is nice for creating diagrams.
- [GitHub](https://github.com/) is where people go to share code.
- [Google](www.google.com) is where you go when you don't know something.
- [StackOverflow](https://stackoverflow.com/) is where Google will bring you
when you don't know something.

### Command Line
Learning to use the command-line interface is absolutely mandatory. If you're
using a Mac or Linux, the basic terminal is what you want. If you're on Windows,
set up [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install-win10) first, which will
basically let you pretend like you're using Linux on your machine.
- [Terminus](http://web.mit.edu/mprat/Public/web/Terminus/Web/main.html) is a
fun web game from MIT that will help you get your feet wet.
- [The Linux Command Line](http://linuxcommand.org/tlcl.php) book is a great,
structured way to learn what you can do with the command line.

### Text Editors
I recommend using a text editor rather than an IDE (Eclipse, RStudio, etc.).
You'll need to learn a new IDE for each new language you learn, whereas one
good text editor can serve all your coding needs.
- [Emacs](https://www.gnu.org/software/emacs/) does everything, if you're
willing to write enough LISP (!) to make it happen. Emacs is 42 years old.
- [Vim](https://www.vim.org/) is another ancient text editor for hardcore
coders. Customized using another weird language: Vimscript.
- [Sublime Text](https://www.sublimetext.com/) is a friendly Python-based
editor designed for humans, but it isn't free :(  
- [Atom](https://atom.io/) is relatively new and caters more to the Sublime
crowd. Based on CoffeeScript, a variant of JavaScript
- [VS Code](https://code.visualstudio.com/) is like Atom, but from Microsoft.
Independent from the IDE, and free. Runs on all operating systems.

### Markup Languages
- [Here](https://www.math.hmc.edu/computing/support/tex/classes/hmcpset/) is a
LaTeX class file to make your homework assignments look nice and professional.
- This [Norwegian LaTeX table editor](http://truben.no/table/) has saved my
bacon several times.
- [The Markdown Syntax
Page](https://daringfireball.net/projects/markdown/syntax) is occasionally
useful.
___
## Programming Languages
### [Python](https://www.python.org/)
Use Python unless you have a good reason not to.
- Install with [Anaconda](https://www.anaconda.com/download/), or its smaller cousin,
[Miniconda](https://conda.io/miniconda.html). Never use the basic installer.
- [Jupyter Notebooks](http://jupyter.org/) are how most people share their data
science work. Plays nice with GitHub.
- [Automate the Boring Stuff with Python](https://automatetheboringstuff.com/)
(free) might be the world's best introductory programming book.
- [Friendly tutorial videos on YouTube](https://www.youtube.com/user/sentdex)
to get started.
- [PyCon](https://www.youtube.com/channel/UCrJhliKNQ8g0qoE_zvL8eVg),
[PyData](https://www.youtube.com/channel/UCOjD18EJYcsBog4IozkF_7w), and
[SciPy](https://www.youtube.com/user/EnthoughtMedia/playlists) talks for more
advanced stuff and to learn about new packages.

### [R](https://www.r-project.org/)
Used by statisticians. Arguably the nicest language to work with data in. Also
arguably not a real programming language.
- Using R without [Tidyverse](https://www.tidyverse.org/) should be illegal.
- [Advanced R](http://adv-r.had.co.nz/) for when you're ready for hard stuff.
- Many R people like to use [R-Studio](https://www.rstudio.com/) as their IDE.
I'm not a fan.

### Other
- C++ is used in packages that require heavy computation, frequently with a
Python interface.
- Java and Scala are used for managing massive datasets.
- JavaScript is king for web-based data visualizations.
___
## Databases
100% of people who manage databases are familar with
[SQL](https://www.w3schools.com/sql/default.asp). Get some practice with
SQL by using [SQLite](https://docs.python.org/3/library/sqlite3.html),
which comes with Python.

Beyond that, I'm told [Hadoop](http://hadoop.apache.org/) and
[Spark](https://spark.apache.org/) are important. (This section could
use a contribution from someone who knows this stuff.)
___
## Data Visualization
Data visualization is useful not only for presenting the results of an
analysis, but also for exploring data before creating mathematical models.
Advanced data visualization tends to bleed into front-end web development and
computer graphics.
### Data Visualization Software
- [Matplotlib](http://matplotlib.org/) for simple plots guaranteed to work
everywhere.
- [Seaborn](http://seaborn.pydata.org/) lives on top of Matplotlib and makes
common plotting tasks easy.
- [Bokeh](http://bokeh.pydata.org/en/latest/) for interactive and web-based
plotting.
- [Datashader](http://datashader.readthedocs.io/en/latest/) for plotting
large datasets.
- [Altair](https://altair-viz.github.io/) for when you miss ggplot-ing (see next).
- [Plotly](https://plot.ly/) is similar to Bokeh. Also commonly used from R.
- [ggplot2 (R)](http://ggplot2.org/) is the most important plotting package in
R.
- [Shiny (R)](https://shiny.rstudio.com/) for interactive web-based data
visualizations.
- [D3 (JavaScript)](https://d3js.org/) is the go-to library for serious interactive data visualization.

### Data Visualization Books and Links
- [The Visual Display of Quantitative
Information](https://www.amazon.com/Visual-Display-Quantitative-Information/dp/0961392142/ref=sr_1_1) is a classic book, though I'll admit I haven't read it.
- I personally enjoyed [Storytelling with Data](https://www.amazon.com/Storytelling-Data-Visualization-Business-Professionals/dp/1119002257/ref=pd_sim_14_11), which I believe covers similar ground.
- [The New York Times Graphics Team](https://twitter.com/nytgraphics?ref_src=twsrc%5Egoogle%7Ctwcamp%5Eserp%7Ctwgr%5Eauthor) is famously good for making interesting visualizations.
- The [Data Is Beautiful](https://www.reddit.com/r/dataisbeautiful/) subreddit.
- A [free online book](http://jsdatav.is/) about dataviz in JavaScript covering several packages.
___
## Math
Every part of math can be used in data science somehow, but only a few fields
are really essential.
### Calculus
Understand partial derivatives and multiple integrals. Be able to take numerical
integrals (using something like [SciPy](https://www.scipy.org/)). Be able to
"type math" using [LaTeX](https://faculty.math.illinois.edu/~hildebr/tex/latex-start.html).

- [MIT Single Variable Calclus Lectures](https://www.youtube.com/playlist?list=PL590CCC2BC5AF3BC1)
- [MIT Multivariable Calclus Lecutures](https://www.youtube.com/playlist?list=PL4C4C8A7D06566F38)

### Linear Algebra
Know matrix operations inside-out and be able to implement everything on
a computer (using, say, [NumPy](http://www.numpy.org/)). Used in almost
every area of statistics and machine learning.
- I enjoyed [this YouTube series](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)
for visual, intuitive explanations of linear algebra concepts.
- [Linear Algebra and Its Applications](https://www.amazon.com/Linear-Algebra-Its-Applications-4th/dp/0030105676) is a popular resource for this subject.

### Optimization
Any time you need to find the "best" thing, you have an optimization problem.
- [Here](https://web.stanford.edu/~boyd/cvxbook/) is a free, popular book on
convex optimization. This is overkill for most data scientists.

### Probability Theory
Totally mandatory. If you see the phrase "measure theory", *run*.
- [Here](https://www.dartmouth.edu/~chance/teaching_aids/books_articles/probability_book/amsbook.mac.pdf) is a free book on basic probability theory. Doesn't cover
multivariate distributions.
___
## Statistics
Statisticians cared about data before it was cool. Closely related to psychometrics,
econometrics, and other "-metrics".
### Core Concepts
You should probably understand these ideas. In particular, know what a p-value is
and be able to describe it accurately.
- Confidence intervals
- Hypothesis tests
- Generalized linear models

### Bayesian Statistics
- [Bayesian Data Analysis](http://www.stat.columbia.edu/~gelman/book/) is the
most common introduction to the field.
- [Bayesian Nonparametrics](https://www.amazon.com/Nonparametrics-Cambridge-Statistical-Probabilistic-Mathematics/dp/0521513464) for more advanced Bayesian modeling.
- [Stan](http://mc-stan.org/) is probably the most mature package for Bayesian
modeling.

### Time Series
For when your data are related across time.
- [Time Series Analysis](https://www.amazon.com/Time-Analysis-James-Douglas-Hamilton/dp/0691042896) is a great intro- to mid-level reference for the field.
- [Time Series: Theory and Methods](https://www.amazon.com/Time-Theory-Methods-Springer-Statistics/dp/1441903194), despite its name, is mostly theory. Expect heavy math.

### Statistics Software
R is much more popular than Python for classical statistics and has a more
comprehensive package ecosystem.
- [Statsmodels](http://www.statsmodels.org/stable/index.html) for classical
statistics in Python.
- MINITAB, SAS, STATA, and SPSS are probably still used in some places.
___
## Machine Learning
Machine learning is essentially statistics, but hyper-focused on the problem
of making predictions.
### Basics
Don't jump the gun and try to use deep learning without understanding simpler
methods first.
- If you're willing to use R, [An Introduction to Statistical
Learning](http://www-bcf.usc.edu/~gareth/ISL/) is one of the fastest ways to
get up and running with machine learning.
- [Stanford CS 229](http://cs229.stanford.edu/) is Andrew Ng's famous
introductory machine learning course. Videos from a previous semester should
be available on YouTube. Use NumPy; MATLAB is the devil.
- [The Elements of Statistical
Learning](https://web.stanford.edu/~hastie/ElemStatLearn/) is arguably the
"bible" of standard machine learning methods.
- Use [NumPy](http://www.numpy.org/) to implement these algorithms
for yourself to make sure you really understand them.
- [Scikit-learn](scikit-learn.org/) is how you will implement most of these
methods in practice.
- [Spark](https://spark.apache.org/) for large-scale machine learning.

### Neural Networks and Deep Learning
Computation-heavy, data-hungry methods that aim to automate the feature
generation process before doing classification, regression, etc. Popular since
around 2012. Notoriously difficult to interpret. Only use this when easier
methods fail.
- [Neural Networks and Deep Learning](http://neuralnetworksanddeeplearning.com/)
gives a good, clear introduction to deep learning basics. Includes building
neural networks from the ground up using NumPy, then transitions to Theano
(which is outdated; use something more modern).
- The [Deep Learning book](http://www.deeplearningbook.org/) is indeed THE book
on deep learning. This should bring you up to speed with the state of the art
as of about early 2016. Biggest flaw: no exercises.
- [TensorFlow](https://www.tensorflow.org/) for "low-level" neural network
programming.
- [Keras](https://keras.io/) for higher-level programming. Lives on top of TF.
Use this a ton.
- [PyTorch](http://pytorch.org/) for a more friendly but less widely-used
alternative to the TensorFlow stack.
___
## Other Resources
### Blogs
Company engineering blogs tell you about the research they're
doing and the tools they're using. 
- [Google Research Blog](https://research.googleblog.com/)
- [Facebook Research Blog](https://research.fb.com/blog/)
- [DeepMind Blog](https://deepmind.com/blog/)
- [Uber Engineering Blog](https://eng.uber.com/)

Many individuals out there also publish interesting material on their blogs,
or on [Medium](https://medium.com/).


### News
- [ArXiv](https://arxiv.org/) provides new papers every day, for free!
- I didn't want to admit it at first, but [Twitter](https://twitter.com/)
is a great source of ML news.

### Podcasts
I've found data science podcasts to be an enjoyable source of ideas and news
from the data science community.
- [Linear Digressions](http://lineardigressions.com/) and [Partially
Derivative](http://partiallyderivative.com/) are generally less serious and
very friendly for people just entering data science.
- [Talking Machines](http://www.thetalkingmachines.com/) is a great podcast
about machine learning. The first few seasons discuss topics at a very advanced
level, however.
