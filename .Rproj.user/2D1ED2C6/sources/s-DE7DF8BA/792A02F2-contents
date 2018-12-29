---
title: Adstocking, Retention rate and Half Life
author: Aritra Biswas
date: '2018-12-29'
slug: adstocking-retention-rate-and-half-life
categories: []
tags: []
---

In a marketing mix study one of the major hypothesis is that a marketing tactic specially media does not impact immidiatly. There are several factors other than the execusion which impact sales caused by a marketing tactic. Here are some of the important facts associated with media tactics,

* Suppose one tactic has been executated at a point of time. Then amount of time it is remembered to an individual exposed with the advertisement is known as half life. 

* Suppose one tactic has been executated at a point of time. Then it has some carry over impact which goes to the next period of execusion. The amount of impact which has been carry forwared to the next period from the existing period is known as retension rate. 

* Advertisements in two major different period (i.e. FY 2017 and FY 2018) do not have the same amount of effectiveness. For example the same advertiement has signed a more popular actor for 2018 than it had in 2017. Then it is expected that the effectiveness of that advertisement will be more in 2018 in comparison with 2017. This added impact is measure by copy core or effective index. This works like a multiplier with the regression coefficient obtained from the modeling period in the simulation period in order to account for the additional effectiveness of the new camping. 

* Execusion in TV or any other tactics has a snowball kindoff effect due to the presence of retention rate. Although for certain period there is no execusion on a TV tactic but there exists some sort of carry over impact of the advetisement because of the retension rate. The orginal execusion on a marketing tactic is known as causal (GRPs) and the hypothetical carry over impact of the tactic due to the retension rate is know as adstocked causal. 

__Retension rate:__ Renetion rate is a measure which suggests how much impact of a media tactic will be carried forward in the subsequent period of execusion. For example for a weekly level model a retension rate of 0.3 means, in the immidiate sub-sequent week the tactic will bring incremental equivalent to 30% of the existing causal can bring. Retension rate lies between 0 to 1. 0 means that theere will be no carry over of the impact of a tactic and 1 means impact of the tactic will be same accross the sub-sequent weeks. 

In a marketing mix modeling say there are $p$ media variable, then for the $i$ variable retension rate will be denoted as $rr_i$ for further reference purposes.

__Half Life:__ Half life and retension rate are function of one another. Half life means that after how many period of execusion the impact of the tactic will be exactly half. One can clearly see that retension rate and half life are directly depdent upon one another. 

Let us denote half life as $hl_i$ for the $i-th$ media tactic, then the formula for retension rate will be:

$$rr_i \; = 0.5 ^{\frac{1}{hl_i}} \; where \; rr_i \in [0,1]$$


__Adstocked Causal:__ Here for refence purpose we will use $c_t$ for causal at the time period t and $ac_t$ for adstcked causal at execusion period $t$. For a execusion period $t$ Adstocked causal can be calculated by using the following formula:

__Simple addtive model adstock:__  

This is the most popular for of the adstocking in current practise for addtive models. Using recurssion one can easliy derive the following result:

$$ac_{it} \; = c_{it} + ac_{i(t-1)} \times  rr_i$$  

$$ac_{it} \; = c_{it} + (c_{i(t-1)} + ac_{i(t-2)} \times  rr_i) \times  rr_i$$  

$$\dots$$  

$$ac_{it} \; = \sum_{T=0}^{t} rr_i^{T-i} \times ac_{i(t-T)}$$  

In case of a logaritmmic model here is the following transformation which has is used:


__Logarithmic adstocking:__

$$ac_{it} \; = log(c_{it}) + ac_{i(t-1)} \times  rr_i$$  


__Negative exponential adstocking:__

$$ac_{it} \; = (1 - \exp(- shape \times c_{it})) + ac_{i(t-1)} \times  rr_i$$  

__S-curve adstocking:__

$$ac_{it} \; = \frac{1}{(1 + \exp(- shape \times c_{it}))} + ac_{i(t-1)} \times  rr_i$$



Here in this following section we will code this formula in R and Python in order get out hands dirty. We will try to understand the nature of these adstocking by visualization and looking at their symmary statistics and try to infer that how does that impact out analysis further in the modeling and planning stage. 

