---
layout: infolab-toplevel
title: Dashboards
permalink: /dashboard/
header:
  overlay_image: /assets/images/water.jpg
  overlay_filter: "0.7"
toc: True
---

<div class='tableauPlaceholder' id='viz1750087120068' style='position: relative'>
  <noscript>
    <a href='#'>
      <img alt='Dashboard 1' src='https://public.tableau.com/static/images/77/77FQMF6S9/1_rss.png' style='border: none' />
    </a>
  </noscript>
  <object class='tableauViz' style='display:none;'>
    <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
    <param name='embed_code_version' value='3' />
    <param name='path' value='shared/77FQMF6S9' />
    <param name='toolbar' value='yes' />
    <param name='static_image' value='https://public.tableau.com/static/images/77/77FQMF6S9/1.png' />
    <param name='animate_transition' value='yes' />
    <param name='display_static_image' value='yes' />
    <param name='display_spinner' value='yes' />
    <param name='display_overlay' value='yes' />
    <param name='display_count' value='yes' />
    <param name='language' value='en-US' />
  </object>
</div>

{% raw %}
<script type='text/javascript'>
  var divElement = document.getElementById('viz1750087120068');
  var vizElement = divElement.getElementsByTagName('object')[0];
  if (divElement.offsetWidth > 800) {
    vizElement.style.width = '100%';
    vizElement.style.height = '4027px';
  } else if (divElement.offsetWidth > 500) {
    vizElement.style.width = '1200px';
    vizElement.style.height = '6027px';
  } else {
    vizElement.style.width = '100%';
    vizElement.style.height = '3577px';
  }
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>



## The PolarVis Social Media Dashboard 


A key contribution of the PolarVis research project is the development and design of a Social Media Dashboard to compare different visual climate communication strategies. The dashboard is an interactive tool that empowers website visitors to explore data on social media posts. It enables users to understand the impact of posts on audiences, evaluate the performance of specific posts over time, and compare communication strategies used by various climate change actors.

<img align="center" width="1100" src="/assets/images/dashboard3.png" />



<br />


## The PolarVis Election Dashboard 

This interactive dashboard visualizes and analyzes social media dynamics related to climate change messages featuring visual content, published in the lead-up to the 2021 German federal election. It explores a dataset of approximately 84,000 social media posts from Instagram, Facebook, and Twitter, each containing at least one image.

The dashboard was developed by [Tobias Raidl](https://www.linkedin.com/in/tobias-raidl/) as part of the Interdisciplinary Project in Data Science (TU Wien), during which he collaborated with the PolarVis team at the University of Vienna to interpret the key analytical goals of the PolarVis project and create a dashboard that allows users to explore and analyze the data in the most effective way for the intended purposes.

A primary objective of the visualization is to identify instances of image-sharing polarization, where images are shared exclusively within partisan communities. This functionality is achieved through a component of the dashboard consisting of a large network graph, where nodes represent social media accounts. Two accounts are connected if they shared at least one identical image during the six-week period leading up to the election. In addition to a filter option, the graph visualization includes the following interactive features: clicking on a node reveals more information about the corresponding account, while clicking on a connection displays the images shared by both accounts.

<img align="center" width="1100" src="/assets/images/polarisationdashboard.jpg" />

The dashboard also allows identifying instances of image-sharing across partisan lines, where accounts associated with different political parties shared identical images.

<img align="center" width="1100" src="/assets/images/polarisationdashboard2.jpg" />
<img align="center" width="1100" src="/assets/images/polarisationdashboard3.jpg" />

Additionally, the dashboard allows users to track how an image spreads across platforms by following its historical trajectory from one platform to another.

<img align="center" width="1100" src="/assets/images/polarisationdashboard4.jpg" />

<br />


Cases of cross-platform sharing, where the same image is shared on multiple platforms, are further highlighted by a dashboard component consisting of a filterable bar chart that displays the most shared images across selected social media platforms. Clicking on a bar provides detailed information about the image, including its dissemination across different platforms.

<img align="center" width="1100" src="/assets/images/polarisationdashboard5.jpg" />
