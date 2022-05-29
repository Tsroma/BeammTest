---
contact_image: images/vectors/contact.png
draft: false
layout: beamm
title: Creating a synthetic micro-dataset
weight: 2
---

# The objective
The first step consists of building a suitable micro-dataset. The Beamm model needs detailed micro-data (i.e., data on an individual level) allowing it to compute the individual taxes, social security contributions, transfers as well as the socio-economic background information needed to present a detailed impact analysis. 
# Statistical matching  
Because no existing representative dataset covers all the required pieces of information for Belgium, we need to merge different existing datasets, each containing parts of the required information. However, all individuals and households are anonymous in each dataset that we have at our disposal, such that exactly connecting the information from different datasets to the correct individual is impossible. Fortunately, this is also not necessary, because we need our dataset to be correct at an aggregate level, and are not interested in being correct at the level of single individuals. To merge the different datasets into one single synthetic dataset with all the necessary information, we employ advanced statistical matching techniques (machine learing algorithms). 
# The data
The foundation of this synthetic dataset is an administrative dataset covering the entire Belgian population, and containing some key tax data as well as important socio-economic data. To complete the information about socio-economic background, we statistically merge these data with a series of additional datasets: the Survey on Income and Living Conditions (EU-SILC), the Household Finance and Consumption Survey (HFCS), the Household Budget Survey (HBS), the Labour Force Survey (LFS), BELDAM, MONITOR, the time use survey (HETUS), onderzoek verplaatsingsgedrag (OVG) etc. 
Because all individuals in all our datasets are anonymous, the information that we impute from these additionnal surveys into the main dataset will almost always be incorrect at the individual level, but we aim to make this imputation as statistically correct as possible at the level of the population, such that the dataset represents the real world as closely as possible. 
# Simulation of a fictitious dataset  
Once all micro-datasets are integrated, we have a highly realistic and very rich dataset, that may still contain some blocks of real data. For online use in the present interface, we use machine learning algorithms to create an entirely fictitious dataset that is very realistic and gives very similar simulation results as the real dataset, in technical terms: that has the same joint distributions as the 'real' synthetic dataset. This synthetic 100% fictitious but highly realistic dataset is used in the present online simulation platform. 
