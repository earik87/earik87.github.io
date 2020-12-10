---
title: "Interactive Web Application to Visualize Scientific Data"
layout: post
---

When I was a PhD (still a candidate), I collected tremendous amount of data with ultrafast spectroscopy setups. The data is 3-dimensional (time, wavelength, absorbance), and plotting meaningful graphs from it requires extensive - repetitive coding. Other challenge is presenting these figures to my co-workers. Most of the time, I prepared pdfs or even print-outs to discuss the results in the meetings. This way of working is not ideal when a co-worker requests "can you show *this* particular dataset", or "can you zoom in *here*?". Essentially, these things can be easily solved by using interactive dashboards.

In this blog, I will show you the steps on how to create a web application for visualizing a scientific data. 

1. We will create an interactive app.<br>
Instead of plotting static figures, we create an interactive dashboard which visualizes the **full dataset**. 
2. We will deploy the app into the website.<br>
We will serve this dashboard in a website for our co-workers. 

## Creating an interactive dashboard with Panel

The visualized figures must be interactive so that user can easily get into the data itself without extra effort. Here, I am going over an example of 3-dimensional data (time, wavelength, absorbance) which is a typical transient absorption data of Photoactive Yellow Protein. You can plot this whole data set with a heat map (Figure 1). It is nice and neat, however, this comes with a drawback. You miss lots of details, such as spectral shape at certain time points and time-traces at certain wavelengths.

<center>
    <figure>
    <img src="/assets/images/heatmap.png" alt="heatmap" width="400"/>
    <figcaption>Figure 1. Transient Absorption Data demonstrated with heat map. Plotted in Matlab.</figcaption>
    </figure>
</center>

To visualize all the details in this dataset, we essentially need an interactive plot. Possibly with a slider which sets one parameter at a time (time or wavelength) then plot will be updated, accordingly. Two figures side by side can solve our problem; Absorbance vs Time figure and Absorbance vs Wavelength figure. [Panel](https://panel.holoviz.org/) from [Holoviz](https://holoviz.org/) family is a high level app helping people to create interactive figures with few lines of code. You can see the demo below, how the figures are updated in real-time within the use of slider. First section has sliders to show full data set. Note that in the right side of the figures there are buttons which allows you to zoom in/out, save figure, select certain section in the plot etc. Its fully interactive! 

<center>
    <figure>
    <img src="/assets/images/demoinaction.gif" alt="herokudemo" width="600"/>
    <figcaption>Figure 2. Web Application in action.</figcaption>
    </figure>
</center>

## Deploying with Heroku

The app above works in jupyter notebook with python codes. This is fine but everytime you need to go, open jupyter notebook, run all the cells to access the figures. Not a quick workflow. What about if we deploy this app into a website, where people without any programming knowledge can open the figures and use them like a toy? Actually the demo in Figure 2 is recorded from the [website](https://visud.herokuapp.com/) where I deployed the panel-app into. There are several cloud services for deployment  out-there, but I chose Heroku for its easiness. There is an extensive [documentation](https://devcenter.heroku.com/articles/getting-started-with-python?singlepage=true 
) exists on how to deploy python projects to Heroku. Although it has a decent documentation, I ran into some errors in the first trial and decided to use a minimal working example - [minimal heroku app](https://github.com/pyviz-demos/minimal-heroku-demo) provided from Holoviz founders. I would **strongly** suggest starting from this just to see how deployment is done. First, you create heroku account, install git on your computer if you didn't have, and install Heroku Command Line Interface (CLI). You need `heroku login` command for authorization. Then, follow the instructions in the minimal heroku app and voala! <br>

I still have quite few things to-do about this webapp;
- First launch of website takes some time (about 30 seconds). Not sure how to improve this, but I will check.
- The response time of sliders isn't very quick. I think there is a room for optimization on the code to speed-up the figure's responses. Not sure how much the panel app brings slowness due to its high-level infrastructure. 
- Range slider can be added for desired x, y axis range. 
- Linear - logarithmic time-axis should be implemented to access the full time-scale for time-trace plotting. 

I am not sure where I will go from here to be honest. But, I will likely be stick to Panel and Heroku, and try to improve the project. 

Helpful links of this project; 
- [Heroku web app](https://visud.herokuapp.com/)
- [Github Repo](https://github.com/earik87/visualize-ultrafast-data) 

If you are interested in python source code of this app, check out [source file](https://github.com/earik87/visualize-ultrafast-data/blob/master/visud-heroku-app/vis_ultrafast_data.ipynb).

If you have questions or comments about this project, feel free to reach me via [twitter](https://twitter.com/earik87).
