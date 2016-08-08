---
layout: post
published: false
---

<style type="text/css">
.box
{
  border-width: 2px;
  border-color: #000000;
  border-style: solid;
  padding:1px;
  margin-left: auto;
  margin-right: auto;
}
.center-text
{
  text-align:center;
}
.smallpic1
{
  height: 20px;
  width: 20px;
}

</style>

The past month at Metis has been busy, busy, busy. Yesterday we all presented our McNulty projects. Mine used data from the 2012 [National Ambulatory Medical Care Survey](http://www.cdc.gov/nchs/ahcd/index.htm) on visits to physicians for any type of injury or poisoning, and I tried to build a model to predict which injuries had been intentionally self-inflicted. It’s a nationally representative survey of outpatient visits in the U.S., with record weights available to derive national estimates of outpatient visits and their characteristics (e.g., diagnoses given, medications prescribed). The dataset has over 70,000 visit records and 600 variables. I restricted analysis to the ~2,500 injury-related visits and I used no more than 20 variables to build a feature set to predict whether the physician specified that the injury had been intentional or non-intentional. This was a specific question on the visit form that participating doctors filled out for every patient contact during a randomly selected week in 2012. My hunch is that intentional self-injury will not always be identified as such, at least when the injury is mild enough to be treated in an outpatient setting.  I modeled a classifier that identified 79% of the cases of self-injury in a held-out testing dataset. The only way to capture that many of the cases was at the expense of a high false positive rate. 

So far I’ve discovered one machine learning project concerned with non-suicidal self-injurious behavior, at MIT MEDIA LAB (https://www.media.mit.edu/research/groups/1447/valinor-mathematical-models-understand-and-predict-self-harm
). It appears to be in the development stage and seems to be well funded.



![](/images/self-harm/005008-0216-01-eng_clip_image006.gif){: .box }

![](/images/self-harm/Self-injurious%20throughts%20and%20behaviors%2075.png){: .box }


![](/images/self-harm/self-harm cycle_1.jpg){: .box }

![](/images/self-harm/self_harm.png){: .box }
![](/images/self-harm/self-harm-map.png){: .box }


![fireworks1](/images/self_harm_diagram.jpg){: .center-image }

***








