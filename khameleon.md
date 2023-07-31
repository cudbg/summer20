---
layout: page
title: 
---

<style>
.cool {
  background-color: steelblue;
  color: white;
  text-weight: bold;
}
</style>

# Overview




## Khameleon

Khameleon is a new prefetching framework for cloud-based interactive applications. The main idea is to trade off latency for response quality by combining progressive encoded response and resource-aware scheduling.    The paper and screenshots [can be found here](https://drive.google.com/file/d/1753VKeIz_uVHnHFd1VxsGbSD5r2XgM0e/view).

### Project 1. Multi-media Exploration Application

We have already [built a simple demo](https://drive.google.com/file/d/1UwXYxmWAMN9kOb4mdmQuH9EW194BsPOB/view) that lets users explore a big collection of images.  However, it was a custom implementation where we manually encoded the image corpus, loaded it on the server, and built a custom webpage for the demo.  Your project will be one of the following tasks:

1. Generalize our demo into an API that any developer can use to easily set up their own custom image exploration deployment.   Basically, the developer can point to a massive image collection (say, on AWS S3) and write a little bit of front-end code to easily create a custom responsive image exploration app.
2.  Help brainstorm and Build an AWESOME demo that lets users explore a large image and audio collection.  As one possibility, take a look at [http://everynoise.com/](http://everynoise.com), which lets you explore music genres by clicking on each point.  The demo could be similar, in the sense of rendering a large interactive point cloud.  Instead of needing to click on each point, the user can immediately hear audio and see the corresponding high resolution image when she hovers over a point.  The task will involve brainstorming what the demo would exactly be and finding the dataset.

Skills:

* Front-end: typescript/javascript 
* Backend server: familiarity or willingness to learn Rust  (it helps to know an OOP language e.g C/C++, Java)

### Project 2. Extending Khameleon's scheduler to use reinforcement learning

Khameleon's scheduler ([Section 5 of the paper](https://drive.google.com/file/d/1753VKeIz_uVHnHFd1VxsGbSD5r2XgM0e/view)) is basically a degenerate version of reinforcement learning.  We are interested to replace the scheduler with a reinforcement learning-based scheduler.  The challenge is to ensure it runs in real-time (in microseconds).


Skills:

* Background in Reinforcement Learning 
* familiarity or willingness to learn Rust  (it helps to know an OOP language e.g C/C++, Java)


## Precision Interfaces

Precision interfaces (see [short paper (newer)](https://arxiv.org/pdf/2001.01902.pdf) or [full paper (older)](https://www.dropbox.com/s/9i0pbkacqpb5s0r/precisioninterface-sigmod19-cr.pdf?dl=0)) is a research project that uses query logs to automatically generate interactive data analysis interfaces.  For instance, you might do SQL-based analysis in a Jupyter notebook, and the system would generate an interactive visualization interface for the analysis.

### Project 3.  Front-end Engine

The current system generates an abstract interface specification.
The goal of the summer project is to develop our front-end engine.
The engine takes as input a specification, and generates an interactive interface in the browser that the user can use for data analysis.

The basic scaffolding for the engine has been developed, however the details on how it connects to a backend database, how interactions are executed, and the set of widgets and visualizations it supports, all need to be fleshed out.
The goal is to integrate this engine with Precision Interfaces, and embed both into Jupyter Notebook.

Skills:

* Front-end: Javascript, willingness to read JS library source code
* Backend: Python, abstract syntax trees


