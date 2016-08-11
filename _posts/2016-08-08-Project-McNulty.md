---
layout: post
published: true
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
  margin-left: auto;
  margin-right: auto;
}

.medpic1
{
  height: 200px;
  margin-left: auto;
  margin-right: auto;
}

</style>

Yesterday at [Metis bootcamp](http://www.thisismetis.com/data-science-bootcamps), each of us presented our third projects (dubbed 'McNulty'), for which our basic task was to use machine learning techniques to train, test, and assess the prediction performance of a categorical classifier. I chose to use data from the 2012 [National Ambulatory Medical Care Survey](http://www.cdc.gov/nchs/ahcd/index.htm) to see how well I could predict whether an injury or poisoning treated by a physician was intentionally self-inflicted. My hunch is that intentional self-injury will not always be identified as such, at least when the injury is mild enough to be treated in an outpatient setting. The better we can identify patient characteristics associated with a physician assessing an injury as self-inflicted, the better we might be able to inform other physicians--including ones not inclined to suspect self-injury when an injury seems consistent with accidental injury. 



The survey is carefully designed, and rate estimates derived from it are nationally representative of outpatient visits in the U.S. There were over 70,000 medical visits sampled in 2012 (the latest year for which full data were available), and more than 600 variables are [available for public use](http://www.cdc.gov/nchs/ahcd/ahcd_questionnaires.htm). I restricted my analysis to the ~2,500 injury-related visits. Here is the relevant area on the visit form:

![](/images/self-harm/injury_question.png){: .medpic1 }


and I used no more than 20 variables to build a feature set to predict whether the physician specified that the injury had been intentional or non-intentional. This was a specific question on the visit form that participating doctors filled out for every patient contact during a randomly selected week in 2012.  I modeled a classifier that identified 79% of the cases of self-injury in a held-out testing dataset. The only way to capture that many of the cases was at the expense of a high false positive rate. 

So far I’ve discovered one machine learning project concerned with non-suicidal self-injurious behavior, at [MIT MEDIA LAB] (https://www.media.mit.edu/research/groups/1447/valinor-mathematical-models-understand-and-predict-self-harm
). 



![](/images/self-harm/005008-0216-01-eng_clip_image006.gif){: .medpic1}

![](/images/self-harm/Self-injurious%20throughts%20and%20behaviors%2075.png){: .box }


![](/images/self-harm/self-harm cycle_1.jpg){: .box }

![](/images/self-harm/self_harm.png){: .box }
![](/images/self-harm/self-harm-map.png){: .box }



***








