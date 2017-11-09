StarEightyTwo Aeon Machine Learning Predicting Building Water Consumption

[StarEightyTwo](https://www.stareightytwo.org) is a non-profit organization located in the Twin Cities that provides a service for non-profit and government agencies, and allows those interested in learning analytics through project-based work, by providing analytics services free of charge.


## Project Goal

This goal of this project was to assist Aeon, a local non-profit that provides housing to low-income families and individuals, to better predict overall water consumption in the buildings they manage.  The organization maintains a portfolio of 77 buildings, with a wide variety of attributes.  The organization pays for all utilities in the buildings they manage, and one of the challenges they face is occasional high water consumption.  They requested that the members of StarEightyTwo attempt to develop one or more models that would predict expected monthly water consumption, which would allow them to flag buildings having unexpected high consumption levels for investigation.


## Strategy

The strategic approach to the problem was to present it as a one-day team-based modeling challenge.  Prior to the one-day working session, a cleaned dataset would be provided, and three preliminary models would be developed, including a linear model, a time-series model, and a machine-learning model.  These would be presented to the members, along with an overview of the technique chosen.  Members would then select a team for the working session for model refinement.  I was asked by the organizers to take responsibility for leading the machine learning team.

Exploratory analysis of the dataset showed the following characteristics that needed to be managed prior to model construction:
* The data is monthly water consumption by building over a 2-3 year period, which as time-series may be autocorrelated
* Combination of categorical and continuous data
* Many of the continuous variables were not normally distributed
* There were a minimal number of rows with missing data 
* A visual examination of the Spearman correlation coefficient (plotted as a heatmap) shows the autocorrelation in the data
