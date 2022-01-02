---
layout: infolab-toplevel
title: Research
permalink: /research/
header:
  overlay_image: /assets/images/banner.jpg
  overlay_filter: "0.4"
toc: true
---

At the Infolab we do research on all aspects of social data science: we define mathematical *models* to represent contemporary social data, so that it can be processed by computers, we develop computational analysis *methods*, we implement our models and methods in publicly available *software*, and we *apply* them to perform empirical social data analyses. These applications allow us to test our theoretical advances and provide requirements for new developments.

<figure style="width:40%">
<img src="/assets/images/research.png"
         alt="Research process at the Infolab" />
</figure>

## Research areas

### Models and methods for feature-rich networks

<figure style="width:40%">
<img src="/assets/images/ttn.png"
         alt="A temporal text network" />
    <figcaption>A communication network, with actors (A) exchanging messages (M), with timestamps (Vega and Magnani, 2020).</figcaption>
</figure>

Networks have been a popular model to study social systems for longer than one century, and their applicability has increased in the last decades thanks to increased accessibility to social data, for example from online social networks. However, contemporary social data can very heterogeneous, consisting of different types of actors and social ties, multimedia content, and temporal information. In addition, relevant social connections are often not directly available in the data, which implies that we cannot always be certain about which connections exist. Therefore, at the Infolab we study extended network models (also known as *feature-rich*) that can be used to represent the complexity of contemporary social data.

One model we have extensively studied since 2011[^ml-model] are **multilayer networks**. In addition to original research articles, we have also produced material to organise some of the vast knowledge in this area: a [book](http://www.cambridge.org/ge/academic/subjects/computer-science/computing-and-society/multilayer-social-networks?format=PB) on multilayer social networks, [software libraries](/software)[^library] for multilayer network analysis, and survey articles on preprocessing[^simplification], layer comparison[^comparison], community detection[^detection], and diffusion processes[^diffusion]. We have also introduced multilayer network models including textual and temporal information, called **temporal text networks**, and studied measures and algorithms for **probabilistic networks** where edge existence is uncertain.

[^ml-model]: Matteo Magnani and Luca Rossi (2011). <a href="papers/11asonam.pdf" target="_blank">The ML-Model for Multi-Layer Social Networks</a>. International conference on social network analysis and mining (ASONAM). IEEE.

[^library]: Matteo Magnani, Luca Rossi and Davide Vega. <a href="papers/jss.pdf" target="_blank">Multiplex network analysis with R</a>. Journal of Statistical Software.

[^simplification]: Roberto Interdonato, Matteo Magnani, Diego Perna, Andrea Tagarelli and Davide Vega. <a href="http://arxiv.org/abs/2004.14808" target="_blank">Multilayer network simplification: approaches, models and methods</a>. Computer Science Review, Elsevier.

[^comparison]: Piotr Brodka, Anna Chmiel, Matteo Magnani and Giancarlo Ragozini (2018). <a href="papers/18rsos.pdf" target="_blank">Quantifying layer similarity in multiplex networks: a systematic study</a>. Royal Society Open Science, 5(8).

[^detection]: Obaida Hanteer, Roberto Interdonato, Matteo Magnani, Luca Rossi and Andrea Tagarelli. <a href="https://arxiv.org/abs/1910.07646" target="_blank">Community Detection in Multiplex Networks</a>, and C&eacute;cile Bothorel, Juan David Cruz, Matteo Magnani, and Barbora Micenkova (2015). <a href="papers/15NetworkScience.pdf" target="_blank">Clustering Attributed Graphs: Models, Measures and Methods</a>. Network Science 3 (3). Cambridge University Press: 408–44.

[^diffusion]: Mostafa Salehi, Rajesh Sharma, Moreno Marzolla, Matteo Magnani, Payam Siyari, and Danilo Montesi (2015). <a href="papers/15TNSE.pdf" target="_blank">Spreading Processes in Multilayer Networks</a>. IEEE Transactions on Network Science and Engineering 2 (2): 65–83.

### Empirical study of online information networks

<figure style="width:50%">
<img src="/assets/images/pb.png"
         alt="A world map showing the relative frequency of YouTube videos including a given visual theme" />
    <figcaption>A world map showing the relative frequency of top-relevant YouTube videos including a given visual theme in different geographical regions, identified using deep neural network classifiers (Magnani and Segerberg, 2021).</figcaption>
</figure>

Our main application area is the study of online communication. Two current areas of applied research are online disinformation and visual political communication.

Most of the existing computational work on **online disinformation** focuses on a single platform. However, we can expect organised disinformation campaigns and other misinformation spreading processes to happen across platforms. The importance of the content that is spread and the existence of interconnected platforms make online disinformation a timely and appropriate application for our work on feature-rich networks. Some aspects of our interest are: (1) the detection of coordinated behaviors, that is, groups of users or groups of social media accounts collaborating to boost spreading, (2) the role of change of platform in the dynamics of spreading, e.g., to what extent moving from one platform to another (and possibly back) allows reaching new audiences, and (3) the study of how cultural and political conditions of the Nordic countries relate to the observed disinformation processes if compared with other more studied context, e.g., the US. This research is done as part of the Nordic Observatory for Social Media and Information Disorder, of which we are the Swedish academic node.

**Visual content**, such as images, videos, and memes, plays a particularly important role in online communication: it can be persuasive, emotive, and affective, and is widely shared in online environments. For example, visual content plays an important symbolic, emotional and (dis)connecting role in political movements, where it becomes the focus of social and algorithmic negotiation. Part of our research addresses the methodological and empirical challenges related to the study of how visual content propagates online and how it becomes a beacon of political aggregation and polarisation.


## Sponsors

The Infolab is or has been funded by the following projects:

{% for projlist in site.data.projects %}
### {{ projlist.scope }}

{% for proj in projlist.projects %}
**{{ proj.title }}**<br/>
Funding from: {{ proj.funder }}<br/>
Period: {{ proj.years }}<br/>
In short: *{{ proj.description }}*<br/>
{% endfor %}

{% endfor %}


We also thank Uppsala University for providing funding to create the International Master's programme in Data Science (started in the Fall 2020) and our interdisciplinary introductory course on computational social science (first taught in the Spring 2022), and the Division of Computing Science at the Department of Information Technology for continuous support.
