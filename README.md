# Resources
This is an opinionated list of useful resources for data science.

**Q:** I'm a beginner. Where do I go? <br>
**A:** Learn Python and topics in the *Core Math* section below.

**Q:** Do I need to know all of this stuff to be a data scientist?<br>
**A:** No.

**Q:** I don't like math. Can I still be a data scientist?<br>
**A:** I think the core math topics are pretty important, but you can choose to
focus more on the data management side, perhaps with some visualization
tools. Don't expect to do much machine learning, though.

**Q:** I don't like computers. Can I still be a data scientist?<br>
**A:** Not unless you *really* like math.

**Q:** I want to add to this list. Can I?<br>
**A:** Yes. Please be civilized and use pull requests.
___
## General Computing
Perhaps the best piece of advice I ever received about how to improve my
computing skills (not necessarily programming) was that I should install some
variety of Linux, such as [Ubuntu](https://www.ubuntu.com/) (using
[VirtualBox](https://www.virtualbox.org/)) and tinker with it. Once I did that,
I made an effort to use the *command line as much as possible*, simply because
that felt like the right way to begin to dig into more advanced material.
- [Atom](https://atom.io/) is a decent text editor which can be used no matter
which language you prefer to code in.
- [Draw.io](https://www.draw.io/) is what I use to create diagrams.
- [The Linux Command Line](http://linuxcommand.org/tlcl.php) book is a great,
structured way to learn what you can do with the command line.
- [GitHub](https://github.com/) is where people go to share code.
- [Google](www.google.com) is where you go when you don't know something.
- [StackOverflow](https://stackoverflow.com/) is where Google will bring you
when you have computer questions. Also see sister sites
[Cross Validated](https://stats.stackexchange.com/) and the [Data Science Stack
Exchange](https://datascience.stackexchange.com/).

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
Here I provide resources for commonly-used languages in data science. Most links
to specific packages come in later sections.
### Java
Not very widely-used in data science, but possibly useful for dealing with "big
data". The data management tools described in the next section are almost
exclusively programmed in Java or Scala.

### JavaScript
The only language your web browser understands. Used exclusively for
data visualization. Unrelated to Java.
- The [Mozilla Developer Network](https://developer.mozilla.org/en-US/) has
documentation for JavaScript and other related web technologies such as
(HTML and CSS).

### [Python](https://www.python.org/)
Widely used for everything where JavaScript isn't king. Fast to develop in.
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
A domain-specific language for statistics. Many of the Python packages I mention
here have R equivalents, or have their functionality baked into the core R
language by default. Arguably the nicest language to work with data in, at the
cost of flexibility.
- Use [Tidyverse](https://www.tidyverse.org/) packages as much as possible.
- [Advanced R](http://adv-r.had.co.nz/) for when you're ready for hard stuff.
- Many R people like to use [R-Studio](https://www.rstudio.com/) as their IDE.

### [Scala](http://www.scala-lang.org/)
Purpose-built for big data problems. Compatible with Java via the JVM. Has more
functional programming capabilities than the other languaes on this list.
- [ENSIME](http://ensime.org/) provides IDE-like functionality for Scala to
many text editors.
___
## Data Management
### Local Tools
For data that fit in memory, or at least on your hard drive.
- [Pandas (Python)](http://pandas.pydata.org/) for data wrangling.
- [SQLite](https://www.sqlite.org/) creates small, file-sized SQL databases.
- [MySQL](https://www.mysql.com/) for an open-source relational database.
- [Dask](https://dask.pydata.org/en/latest/) can be used when your datasets
don't fit in memory...

### Big Data
For situations where more than one machine may be necessary.
- [Hadoop](http://hadoop.apache.org/) provides a distributed filesystem and an
implementation of the MapReduce method for computing on multiple nodes.
- [HBase](https://hbase.apache.org/) and
[Accumulo](https://accumulo.apache.org/) are databases that play nicely with
Hadoop.
- [Spark](https://spark.apache.org/)
- [Dask](https://dask.pydata.org/en/latest/) ...or when they don't fit on a
single computer...

### Streaming Data
- [Beam](https://beam.apache.org/)
- [Flume](https://flume.apache.org/) is particularly for log data (think log
  flume).
- [Kafka](https://kafka.apache.org/)
- [Spark](https://spark.apache.org/) (again!)
- [Storm](https://storm.apache.org/)

### Workflow Scheduling
(I'm not sure if this really qualifies as part of data science, but it is
frequently mentioned in the context of managing complex data pipelines.)
- [Airflow](https://airflow.apache.org/)
- [Luigi](https://github.com/spotify/luigi)
- [Dask](https://dask.pydata.org/en/latest/) ...or for something else entirely.
___
## Data Visualization
Data visualization is useful not only for presenting the results of an
analysis, but also for exploring data before creating mathematical models.
### Packages
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

### Books and Links
- [The Visual Display of Quantitative
Information](https://www.amazon.com/Visual-Display-Quantitative-Information/dp/0961392142/ref=sr_1_1) is a classic book, though I'll admit I haven't read it.
- I personally enjoyed [Storytelling with Data](https://www.amazon.com/Storytelling-Data-Visualization-Business-Professionals/dp/1119002257/ref=pd_sim_14_11), which I believe covers similar ground.
- [The New York Times Graphics Team](https://twitter.com/nytgraphics?ref_src=twsrc%5Egoogle%7Ctwcamp%5Eserp%7Ctwgr%5Eauthor) is famously good for making interesting visualizations.
- The [Data Is Beautiful](https://www.reddit.com/r/dataisbeautiful/) subreddit.
- A [free online book](http://jsdatav.is/) about dataviz in JavaScript covering several packages.
___
## Mathematical Data Analysis
Most data analyses involve creating *mathematical models* of the processes that
generated the data. With these in hand, the analyst can then make statements
about how those processes operate, make predictions about future data values,
etc.
### Core Math
Basically every branch of math is related to data analysis in some way,
but of course some subjects are more widely-used than others. When learning
math, *do exercises*. You cannot be sure that you understand the material
unless you do; it's *very easy* to trick yourself into thinking you understand
something you don't.
#### Calculus
Understand partial derivatives and multiple integrals. Be able to take numerical
integrals (using something like [SciPy](https://www.scipy.org/)). Be able to
"type math" using [LaTeX](https://faculty.math.illinois.edu/~hildebr/tex/latex-start.html).

- [MIT Single Variable Calclus Lectures](https://www.youtube.com/playlist?list=PL590CCC2BC5AF3BC1)
- [MIT Multivariable Calclus Lecutures](https://www.youtube.com/playlist?list=PL4C4C8A7D06566F38)

#### Linear Algebra
Linear algebra comes in two flavors: "matrix algebra", which deals with arrays
of numbers, and a more advanced, abstract type that builds on it. Matrix
algebra is absolutely mandatory; the more of it you know, the better. The
abstract version is not as important when starting out, but may be useful later
on. When learning matrix algebra, make sure that you're able to implement these
methods on a computer (using, say, [NumPy](http://www.numpy.org/)). Essentially
all statistics and machine learning methods are implemented on a computer using
matrices and vectors.
- I enjoyed [this YouTube series](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)
for visual, intuitive explanations of linear algebra concepts.
- [Linear Algebra and Its Applications](https://www.amazon.com/Linear-Algebra-Its-Applications-4th/dp/0030105676) is a popular resource for this subject.

#### Optimization/Mathematical Programming
Once you have a general form for a mathematical model (perhaps with some
unspecified parameters), you'll then want to know how to nail down the best
one. Any time you need to find the "best" thing, you have an optimization problem. Know what linear and convex optimization problems are, and why they're nice, basic iterative optimization algorithms, etc.
- [Here](https://web.stanford.edu/~boyd/cvxbook/) is a free, popular book on
convex optimization. This is overkill for most data scientists.

#### Probability Theory
There is always uncertainty in how to specify the data-generating process.
Probability is the way to translate uncertainty into mathematical language.
Therefore, making good data models requires you to be familiar with expressing
uncertainty using probability. Understand joint and conditional probability
density functions, common distributions (especially the multivariate normal), the law of large numbers, the central limit theorem, etc. Measure theory is not required.
- [Here](https://www.dartmouth.edu/~chance/teaching_aids/books_articles/probability_book/amsbook.mac.pdf) is a free book on basic probability theory. Doesn't cover
multivariate distributions.

### Statistics
Statisticians are the original data scientists. Related fields include
biometrics, econometrics, psychometrics, etc., which use the same fundamental
tools but use different terminology.
- Bayesian Statistics
- Experimental Design
- Hierarchical Models
- Spatial Statistics
- Survival Analysis
- Time Series

### Machine Learning
Machine learning, a branch of artificial intelligence, has been around since
the 1950s, but for much of its history was essentially unrelated to data
analysis. *Statistical machine learning*, which is now by far the dominant
variety, phrases "learning problems" in the context of data analysis. Like the
\*metrics, expect a lot of similarities to statistics, but with differing
focuses and terminology.
- Unsupervised Learning
- Supervised Learning
- Reinforcement Learning
- Recommender Systems

### Useful Packages
- [Scikit-learn](scikit-learn.org/) for small-scale machine learning
- [Statsmodels](http://www.statsmodels.org/stable/index.html) for classical
statistics

### Computationally Intensive Method Packages
Includes packages for deep learning, as well as other methods that cause
problems for base R and Python.
- [TensorFlow](https://www.tensorflow.org/) for "low-level" neural network
programming. Rarely use this directly.
- [Keras](https://keras.io/) for higher-level programming. Lives on top of TF.
Use this a ton.
- [Edward](http://edwardlib.org/) for the Bayesians. Lives on top of TF. Plays
nice with Keras.
- [PyTorch](http://pytorch.org/) may be fun to play with. Unrelated to TF.
- [Stan](http://mc-stan.org/) for Bayesian modeling. More mature and popular,
but probably less powerful, than Edward.
- [Spark](https://spark.apache.org/) for distributed, non-neural network machine
learning.

### Books
- [The Elements of Statistical
Learning](https://web.stanford.edu/~hastie/ElemStatLearn/) is a good, though
slightly dated book, about machine learning from the statistician's perspective.
I think this book is important to read if you want to understand the motivation
behind many of the most popular ML algorithms.
- [Information Theory, Inference, and Learning
Algorithms](http://www.inference.org.uk/mackay/itila/) is an interesting book
that, as its name implies, explores the relationship between Information (and
  Coding) theory and Bayesian machine learning.
___
## Software Engineering Practices
It is common to hear of recent physics or statistics graduates who decide
to move into data science, only to be assaulted with terms such as "production
code", "unit tests", "logging", etc. These concepts are essential for real
developers but less relevant to researchers.
___
## Other Resources
### Staying Current
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
