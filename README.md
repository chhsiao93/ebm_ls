# ebm_ls
Using EBM to predict the lateral spreading occurrence during the Christchurch Earthquake event

# Data
`data_10m.csv` is the collection of interpreted CPT data (i.e., Ic and qc1ncs) of 12822 CPT sites. We've excluded the sites of which penetration detph doesn't exceed 10 meter, and we take the average of Ic and qc1ncs every 20 centimeter. Each row contains 101 values, including one Test ID for the site, 50 averaged values for Ic, and 50 averaged values for qc1ncs.

`data.csv` is the collection of event specific features of 7291 sites during Christchurch Earthquake event. 
The data indludes: 
<li>GWD - Event specific groundwater depth (meter)
<li>Elevation - Event specific elevation from DEM (meter)
<li>L - distance to Avon river (km)
<li>L_new - distance to rivers, streams, creeks, and wetlands (km)
<li>Slope - slopes computed from DEM data (%)
<li>PGA - Estimated median peak ground acceleration from Bradley (2014) (g)
<li>Target - boolean values for lateral spreading occurence. The occurence is based on the remote-sensing measured displacement with a threshold of 0.3 m
