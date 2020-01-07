---
layout: project
type: project
image: images/RhizobiaMatchResult.png
title: Matching Template with K-Means for Rhizobia Nodes Detection
permalink: projects/matchingRhizobia
# All dates must be YYYY-MM-DD format!
date: 2019-12-01
labels:
  - Image Processing
  - K-Means
  - Python
  - Rhizobium 
summary: A small project to detect rhizobium nodes in legumes roots using OpenCV and K-Means.
---

<div class="ui small rounded images">
  <img class="ui image" src="https://raw.githubusercontent.com/Diolante/Matching-Template-with-K-Means-for-Rhizobia-Nodes-Detection/master/Exp.1%20-%20Florest%C3%B3polis%2C%2035DAE%2C%202017-2018%2C%20T15%2C%20R1%2C%20P2.jpg">
  <img class="ui image" src="https://raw.githubusercontent.com/Diolante/Matching-Template-with-K-Means-for-Rhizobia-Nodes-Detection/master/Exp.1%20-%20Florest%C3%B3polis%2C%2035DAE%2C%202017-2018%2C%20T22%2C%20R5%2C%20P3.jpg">
  <img class="ui image" src="https://raw.githubusercontent.com/Diolante/Matching-Template-with-K-Means-for-Rhizobia-Nodes-Detection/master/Exp.2%20-%20Florest%C3%B3polis%2C%2035DAE%2C%202017-2018%2C%20T4%2C%20R2%2C%20P4.jpg">
</div>

It is a small project, designed to match rhizobia nodes in a given image through a pre-select match template image, where the application return a list of node-locations that the match template algorithm detected, however some of then are not rhizobia nodes, to fix that, we use K-Means to reduce to number of matchs in same locations and to discard outside hits of matching template algorithm.



