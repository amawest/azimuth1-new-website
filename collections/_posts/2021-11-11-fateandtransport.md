---
layout: post
title: Comparing Machine Learning and Fate and Transport Models
description: Tackling some of the most common questions we get about our ML approach in relation to traditional fate and transport modeling applications
date: 2021-11-11
authors: ["Anna Harrington"]
folder: blog/assets/2021-11-11-fateandtransport
thumbnail: "blog/assets/2021-11-11-fateandtransport/header.png"
image: "blog/assets/2021-11-11-fateandtransport/header.png"
categories: ["Machine Learning"]
---

We get questions all the time about how our [EnviMetric](https://www.azimuth1.com/envimetric) model compares to traditional hydrogeology fate and transport models. Let's dive into what each of them are, how they differ, and when to use one vs the other, or both, to gain a better understanding of your site in the time frame and budget you're looking for. At the end we'll share some helpful resources so you can learn more. Environmental site modeling is used across the remediation industry to lower life cycle costs and cleanup times of contaminated sites.  Models help environmental professionals maximize the effectiveness of their remediation approach and get sites to closure.  

## About fate and transport models
Fate and transport models are representations of complex hydrogeologic systems and the migration of chemicals within them.  They simulate the movement of contaminants by advection, diffusion, and dispersion, alterations of chemicals within the subsurface by biological or physical processes, and the removal or release of these chemicals by sorption or desorption (Ohio EPA).

![I1]({{site.url}}/{{page.folder}}/fateandtransport.png){:class="img-fluid" width="80%"}

Fate and transport numerical models solve partial differential flow or solute transport equations through approximations using matrix algebra and discretization of the modeled terrain (either finite difference or finite element).  The model uses grid cells to represent the hydrogeologic environment and simulates a time series.  The success of a fate and transport model relies heavily on the input data—the more extensive the input data set, the more accurate the model’s simulation will be (Ohio EPA).  The best applications of fate and transport modeling occur when the system is very complex and there is sufficient data to input into the model.  Fate and transport models are less applicable in situations where there is not a sufficient data set.

![I2]({{site.url}}/{{page.folder}}/fateandtransport2.png){:class="img-fluid" width="80%"}

## About machine learning models
Machine learning is a branch of artificial intelligence which focuses on the use of data and algorithms to imitate the way humans learn, gradually improving its accuracy. A large data set is collected and standardized, then the model is given the chance to learn from the data set and make predictions about other scenarios based on what it has learned from observing the training data set.

![I3]({{site.url}}/{{page.folder}}/ml.png){:class="img-fluid" width="80%"}

To develop EnviMetric, we compiled and augmented a database containing the findings from thousands of contaminated site investigations and then applied a machine learning model.  By applying machine learning to the knowledge gained from thousands of previous site investigations, we can leverage thousands of observations to then predict contaminant dispersion at uncharacterized sites.


The machine learning algorithm is trained using subsets of the database containing similar sites; the algorithm then produces a statistical prior probability model automatically.    The algorithm’s purpose is not to predict exactly the resulting contaminated zone, but to provide the weight of evidence from many previously observed cases, and serve as a starting point for further refinement, reducing uncertainty and providing confidence bounds on the extent or source of a known contaminant.  Using many observations serves to filter out variation and determine there are consistent migration patterns that can be used to guide a site investigation.

![I5]({{site.url}}/{{page.folder}}/ml3.png){:class="img-fluid" width="80%"}

The EnviMetric model can output two results- an unknown source model and an unknown destination model.  The unknown destination model shows the highest probability estimated for the location of the farthest detectable contaminated area down hydraulic gradient from the source zone.  The second output is the unknown source model.  This is for situations where contamination is detected, but the source of the contaminant is unknown.  This often occurs when one property is contaminated, while a neighboring property may be the source of the contamination.


## Machine learning vs fate and transport: pros and cons

![I6]({{site.url}}/{{page.folder}}/procon.png){:class="img-fluid" width="80%"}


**Interested in trying out EnviMetric?** [**Get started today!**](https://www.azimuth1.com/envimetric-insights.html)

## Some resources to check out
### Fate and transport software options:

- [Groundwater Modeling System (GMS)](https://www.aquaveo.com/software/gms-groundwater-modeling-system-introduction): a groundwater modeling interface based upon MODFLOW

- [MODFLOW and MODPATH](https://www.usgs.gov/mission-areas/water-resources/science/modflow-and-related-programs?qt-science_center_objects=0#qt-science_center_objects): USGS’s modular hydrologic modeling tool for predicting groundwater conditions

- [BIOSCREEN](https://www.epa.gov/water-research/bioscreen-natural-attenuation-decision-support-system): for simulating natural attenuation remediation of dissolved hydrocarbons

- [BIOCHLOR](https://www.epa.gov/water-research/biochlor-natural-attenuation-decision-support-system): for simulating natural attenuation remediation of dissolved solvents


### For more info on ML:

- [KD Nuggets Blog](https://www.kdnuggets.com/)

- [AWS Machine Learning blog](https://aws.amazon.com/blogs/machine-learning/)

- [Github machine learning repositories](https://github.com/search?o=desc&q=topic%3Amachine-learning+&s=stars&type=Repositories&utf8=%E2%9C%93)


### For more info on fate and transport:

- [Colorado School of Mines Integrated Groundwater Modeling Center](https://igwmc.mines.edu/)

- [Ohio EPA Ground Water Flow and Fate and Transport Modeling Guidance Doc](https://www.epa.state.oh.us/portals/28/documents/TGM-14_final1107W.pdf)

- [USGS Modeling Software homepage](https://water.usgs.gov/software/)



**Interested in hearing more from us? [Subscribe](https://www.azimuth1.com/envimetric-insights.html) to our mailing list so you never miss an update!**
