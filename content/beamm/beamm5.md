---
contact_image: images/vectors/contact.png
draft: false
layout: beamm
title: Behavioral modelling
weight: 6
---

# Why behavior?
The tax-benefit micro-simulation model itself does not account for any behavioral reactions of citizens w.r.t. changes in the tax-benefit system. It merely applies the rules of the tax-benefit system, and computes as such the 'day after effect' of a reform, i.e., the impact before citizens can adapt their behavior to the reform. This is not only unrealistic, but changing the behavior of citizens is often an important motivation of policy reforms.  In order to evaluate a policy reform whilst taking behavioral reactions of citizens into account, Beamm must be connected with behavioral models. 
# How does Beamm integrate behavior?
The integration of behavioral models with Beamm is conceptually relatively straightforward. The integration occurs principally at the level of the micro-data, and proceeds in the following steps: 
1. The policy reform is translated (possibly with the help of Beamm) into changes in disposable incomes, generalized costs and other key parameters of the behavioral models. 
2. The behavioral model then operates separately from the tax-benefit microsimulation model to produce predictions in terms of behavioral changes in mobility for different profiles of citizens. 
3. These behavioral predictions are then brought to the synthetic micro-data:  the model reconsiders for each individual in our synthetic micro-dataset the behavior in light of these predictions, and changes the information about mobility accordingly if necessary. 
4. After changing the synthetic micro-data to fit with our behavioral predictions, we apply all the rules of the reformed tax-benefit system on the altered micro-data, and compute for each individual all the transfers and taxes. 
Bringing all this together, the model then presents an analysis and visualization of the impact of the reform from a variety of viewpoints, this time taking the behavioral reactions of people to the reform into account. 
# What behavioral models?
Tax-benefit microsimulation models are very flexible in terms of their integration with behavioral models. At present, CAPE has integrated 3 sorts of behavioral models in the Beamm platform.
- Labor market model: an econometric model of how individuals adapt their labor market participation in function of changes in the tax-benefit system.   
- Consumption model: an econometric model of how individuals and households adapt their consumption patterns in function of changes in prices and disposable (i.e., net) income.   
- Transport models (transport-beamm platforms only): models built by transport engineers to predict how changes in prices (e.g., due to taxes or subsidies) changes how people move by car, public transport, bicycle etc. 