Project spec:

Choose a real-world phenomenon that can be measured and for which you could
collect at least one-hundred data points across at least four different variables.
- Investigate the types of variables involved, their likely distributions, and their
relationships with each other.
- Synthesise/simulate a data set as closely matching their properties as possible.
- Detail your research and implement the simulation in a Jupyter notebook – the
data set itself can simply be displayed in an output cell within the notebook.


Real-world phenomena-

Weather - met.ie for dataset examples to base synthesisation. things like, month v rainfall, sunshine hours, soil temperature 
Pollution - new pollution stations data - investigate
Fatigue cycling of materials? stress ranges v cycles to failure (not sure how that is distributed). Overall logarithmic relationship between stress range and cycles to failure but what is distribution of repeated tests at same stress range?
Electricity usage for a home v weather (sunshine/time of year etc) - use unit usage and met data as above? 
Wind/storm events v geographic location - may be rayleigh distributed here. Perhaps look at buoy data from met.ie and see what relationships are.

Task 1 - investigate above and see what would be interesting to use
        - have downloaded Athenry met.ie observation station data - hourly (which is the smallest discretisation)
Task 2 - do some plotting of the real world data and see what distributions are for chosen phenomena (research what the distribution is). 
        - plan to take 1 year and plot this for some of the variables
Task 3 - decide on variables to synthesise and implement numpy random distributions as appropriate
Task 4 - Plot data



Update: there aren't high correlation values between the parameters - the highest is rainfall v pressure.  Because rainfall is an exponential distribution, it's more meaningful to plot linear regression between the log of rainfall and pressure. It's obvious that there is a very high degree of spread with the data but at least an attempt can be made to generate random data based on the correlation and perhaps random data based on the distribution alone but season based.
