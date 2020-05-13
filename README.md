# Python-SIR-model-for-Influenza-California-
SIR model made in Python to simulate the development of Influenza disease in California with no considered complexities (vaccines, or mutations for example).

My set of variables are:
Number of susceptible people (people that can get sick or not)-> Discrete Quantitative Variable<br>
Number of Removed people (people that got better or died)-> Discrete Quantitative Variable<br>
Number of Infected people (people that are sick)-> Discrete Quantitative Variable<br>
Parameters of the model:<br>
b stands for infection rate (probability that a interaction infected-susceptible will lead to a contagion)<br>
k is the percentage of infected people that will either recover or die.<br>
The values of b and k were defined as established by Mahaffy (2018). The value of b is 0.039928 and k is 0.03517<br>
I defined my population S[0] as 38 (million) because that is California's estimated population (39.6 million- Source: United States Census Bureau estimates 2018) minus the number of ill people that will be explained below. <br>
I defined my number of infected people as 2 (million) because that is a integer that most closely reflects the information I found on CDC (https://www.cdc.gov/flu/weekly/index.htm)<br>
The illness:Influenza (flu) is a contagious respiratory illness caused by influenza viruses that can present severe or mild symptoms (CDC,2019).<br> My model will use the following differential equations:<br>
dS/dt=-bS(t)I(t)<br>
dI/dt=(bS(t)-k)I(t)<br>
dR/dt=kI(t)<br>
