---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi! Thank you for visiting my website. I am a graduate student studying Robotics at the University of Pennsylvania. I am currently in my final semester actively looking for job opportunties in computer vision and motion planning roles. 

In my professional career, I have worked as an integration lead at [SkyMul](https://skymul.com/) (based in Atlanta) and developed end-to-end software pipelines to semalessly integrate with their quadrupedal hardware platform. I have extensively worked with ROS. Before joining Penn, I also worked on feature development for mobile robots for [Mowito](https://www.mowito.in/) which is a robotics startup based out of India. 

I am interested in working towards the holistic development of autonomous mobile robots with an aim to build robust software pipelines to seamlessly work with the given hardware.

Projects
======

Robust cone detection using Lidar and camera
------
The aim of this project is to fuse cone detections from both the sensors and use them to increase robusness. This project is currently a work in progress. We have completed the calibration aspect and seperate cone detection pipelines. We have also overlayed the detections from the camera using YOLO-v7 to filter out the point cloud data. The ultimate aim is to use this robust and fused pipeline to perform SLAM using cone as landmarks. Please check out the current reults below.

<!-- <iframe src="https://www.youtube.com/embed/AknzieI0od0" style="width:200px; height:100px !important;" frameborder="0"></iframe> <iframe src="https://www.youtube.com/embed/5mYCOwyy4mo" style="width:200px; height:100px !important;" frameborder="0"></iframe> -->

<!-- [![Watch the video](https://i.imgur.com/vKb2F1B.png)](https://youtu.be/vt5fpE0bzSY)[![Watch the video](https://i.imgur.com/vKb2F1B.png)](https://youtu.be/vt5fpE0bzSY) -->



<div class="box">
  <iframe src="https://www.youtube.com/embed/AknzieI0od0" frameborder="0" scrolling="no" width="10%" height="2" align="left"> </iframe>
</div>

<div class="box">
  <iframe src="https://www.youtube.com/embed/5mYCOwyy4mo" frameborder="0" scrolling="no" width="10%" height="2" align="right"></iframe>
</div>


<!-- <div align="left">
      <a href="https://www.youtube.com/watch?v=5yLzZikS15k">
         <img src="https://img.youtube.com/vi/5yLzZikS15k/0.jpg" style="width:30%;">
      </a>
      <a href="https://www.youtube.com/watch?v=5yLzZikS15k">
         <img src="https://img.youtube.com/vi/5yLzZikS15k/0.jpg" style="width:30%;">
      </a>
 </div>  -->
<!-- <div align="center">
      <a href="https://www.youtube.com/watch?v=5yLzZikS15k">
         <img src="https://img.youtube.com/vi/5yLzZikS15k/0.jpg" style="width:50%;">
      </a>
</div> -->
Object detection and instance segmentation
------
Implemented end-to-end object detection and instance segmentation pipelines from scratch. Performed post-processing and analysed performence using MAP metric.

<img src="images/ins1.png?raw=true" width="300" height="300"> <img src="images/ins2.png?raw=true" width="300" height="300">

Two-View and Multi-View Stereo for 3D reconstruction 
------
The aim of this project was to use two view and multiple view images to form a 3D reconstruction of the object of interest.

<img src="images/t1.png?raw=true" width="300" height="300"> 

SLAM using Particle Filter for humanoid Robot
------
This project was focused on doing simultaneous localization and mapping by fusing Lidar and IMU data on a humanoid robot.

<img src="images/s1.png?raw=true" width="300" height="300"><img src="images/result.gif?raw=true" width="300" height="300"> 

<!-- A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful. -->
