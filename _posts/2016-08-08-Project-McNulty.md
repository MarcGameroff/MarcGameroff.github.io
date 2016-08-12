---
layout: post
published: true
---

ROUGH ROUGH ROUGH DRAFT

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
  margin-left: auto;
  margin-right: auto;
  width: 200;
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

.center {
  display: inline-block;
  text-align: center;
  width: 100px;
}

.centerImage
{
text-align:center;
display:block;
}

</style>





Yesterday at [Metis bootcamp](http://www.thisismetis.com/data-science-bootcamps), each of us presented our third projects (dubbed 'McNulty'), for which our basic task was to use machine learning techniques to train, test, and assess the prediction performance of a categorical classifier. I chose to use data from the 2012 [National Ambulatory Medical Care Survey](http://www.cdc.gov/nchs/ahcd/index.htm) to see how well I could predict whether an injury or poisoning treated by a physician was intentionally self-inflicted. My hunch is that intentional self-injury will not always be identified as such, at least when the injury is mild enough to be treated in an outpatient setting. The better we can identify patient characteristics associated with a physician assessing an injury as self-inflicted, the better we might be able to inform other physicians--including ones not inclined to suspect self-injury when an injury seems consistent with accidental injury. 



The survey is carefully designed, and rate estimates derived from it are nationally representative of outpatient visits in the U.S. There were over 70,000 medical visits sampled in 2012 (the latest year for which full data were available), and more than 600 variables are [available for public use](http://www.cdc.gov/nchs/ahcd/ahcd_questionnaires.htm). I restricted my analysis to the ~2,500 injury-related visits. 

<center><img src="../images/self-harm/injury_question.png" alt="" width="300"></center>

The only available patient [features](https://en.wikipedia.org/wiki/Feature_(machine_learning)) that were associated with injury intentionality were age and mental disorder status. Younger patients were significantly more likely to self-injure, as were patients for whom the physician listed at least one [ICD-9-CM mental disorder](https://en.wikipedia.org/wiki/List_of_ICD-9_codes_290%E2%80%93319:_mental_disorders). On the strength of those two features, I was able to develop a classifier that correctly identified 79% of the cases of self-injury in a held-out testing dataset. This is called the [recall](https://en.wikipedia.org/wiki/Precision_and_recall#Recall) rate, which is the percentage of positive cases that were identified as positive. The "price" for achieving that rather high recall rate was very low [precision](https://en.wikipedia.org/wiki/Precision_and_recall#Precision), which means that the classifier also wrongly identified many non-intentional cases as intentional. With a larger dataset and additional features, I hope to be able to improve on precision. 

Since completing my analysis, I've found one machine learning project concerned with non-suicidal self-injurious behavior, at [MIT MEDIA LAB] (https://www.media.mit.edu/research/groups/1447/valinor-mathematical-models-understand-and-predict-self-harm
). 




![](/images/self-harm/005008-0216-01-eng_clip_image006.gif){: .medpic1}

![](/images/self-harm/Self-injurious%20throughts%20and%20behaviors%2075.png){: .medpic1}


![](/images/self-harm/self-harm cycle_1.jpg){: .medpic1}

![](/images/self-harm/self_harm.png){: .medpic1}
![](/images/self-harm/self-harm-map.png){: .medpic1}



***








