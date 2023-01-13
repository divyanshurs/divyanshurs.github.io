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

Professional Experience
======

Skymul (Atlanta) - **Integration Lead**
------

My role at Skymul had been to integrate hardware components and create an end-to-end software pipeline for performing waypoint navigation on a mobile platform. During the period of my internship, I've had the opportunity to learn and interact with hardware and learn how to use software drivers to integrate them into a complete system. I worked mainly on integrating three different hardware platforms with the robot. The aim was to test the accuracy of these sensor platforms and decide the best for the robot’s task at hand.

[<img src="images/in1.gif?raw=true" width="300" height="300">](https://youtu.be/_rudkxJkVwE)
[<img src="images/o1.gif?raw=true" width="300" height="300">](https://youtu.be/0yFySHLm6fA)

Mowito Robotics (Bangalore) - **Robotics Engineer**
------

My work was majorly focused on feature development of this controller for client-specific applications of mobile robots (results of this work are shown below). I was also involved in porting the Maxl controller to ROS2 for benchmarking and making the Maxl controller library independent of ROS.

[<img src="images/m1.gif?raw=true" width="300" height="300">](https://youtu.be/Q3ZjfgWT8YQ)
[<img src="images/m2.gif?raw=true" width="300" height="300">](https://youtu.be/9VXhffuqpYs)

Projects
======

Robust cone detection using Lidar and camera
------
The aim of this project is to fuse cone detections from both the sensors and use them to increase robusness. This project is currently a work in progress. We have completed the calibration aspect and seperate cone detection pipelines. We have also overlayed the detections from the camera using YOLO-v7 to filter out the point cloud data. The ultimate aim is to use this robust and fused pipeline to perform SLAM using cone as landmarks. Please check out the current reults below.

[<img src="images/f1.gif?raw=true" width="300" height="300">](https://youtu.be/AknzieI0od0)
[<img src="images/f2.gif?raw=true" width="300" height="300">](https://youtu.be/5mYCOwyy4mo)

Object detection and instance segmentation
------
Implemented YOLO, SOLO, and Faster-RCNN pipelines for object detection and instance segmentation tasks from scratch. Performed post-processing and analysed performence using MAP metric. [GitHub](https://github.com/divyanshurs/object_detection_and_segmentation)

<img src="images/ins1.png?raw=true" width="300" height="300"> <img src="images/ins2.png?raw=true" width="300" height="300">

Path planning approaches for a planar quadrotor
------
This project was a semester long implementation of several methods implemented for planar quadrotor control as a part of the MEAM 517 (Control and Optimization with learning in Robotics). These methods include MPC, iLQR, LQR to follow a nominal trajectory, and minimum snap trajctory planning in differtially flat space of the quadrotor. Each folder above is the complete implementation of the same. The results for the same are as below.

<img src="images/MPC.gif?raw=true" width="300" height="300"><img src="images/ilqr.png?raw=true" width="300" height="300"> <img src="images/traj_track.gif?raw=true" width="300" height="300"><img src="images/min_snap1.png?raw=true" width="300" height="300">


Two-View and Multi-View Stereo for 3D reconstruction 
------
The aim of this project was to use two view and multiple view images to form a 3D reconstruction of the object of interest. For multi-view stereo the plane sweep algorithm was implemented. [GitHub](https://github.com/divyanshurs/two-view_and_multi-view_stereo)

<img src="images/t1.png?raw=true" width="300" height="300"><img src="images/result.gif?raw=true" width="300" height="300">  

SLAM using Particle Filter for humanoid Robot
------
The aim of this project was to perform particle filter based SLAM using the IMU and the LIDAR data from a THOR-OP Humanoid Robot. The IMU data avaialble was filtered and used with lidar data to perform SLAM. The lidar data is transformed into the map co-ordinates by applying suitable transformations. Based on the paricle filter approach the best particle with maximum correlation is chosen and the log odds of the map is updated. This scan-matching technique is used to update the obstacles in real-time on a gridmap as well as localize the robot in the world. [GitHub](https://github.com/divyanshurs/particle_filter_SLAM_humanoid_robot)

<img src="images/s1.png?raw=true" width="300" height="300"><img src="images/final0.png?raw=true" width="300" height="300"><img src="images/final1.png?raw=true" width="300" height="300"><img src="images/final3.png?raw=true" width="300" height="300">

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
