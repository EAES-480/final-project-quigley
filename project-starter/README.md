Project title
================
by Team name

## Summary

This project evaluates vegetation and groundwater anomalies in Southern Africa from 1982–2024, using a monthly time series. Vegetation condition is represented by NDVI standardied as standardied vegetation index (SVI) and groundwater condition by modeled groundwater levels standardized groundwater index (SGI). Both were standardized using a non-parametric normal scores transformation, so values near zero indicate mean conditions, positive values above-normal, and negative values below-normal.
The overarching questions are what are the structures of the distribution for vegetation and groundwater and are there correlations between them in Southern Africa? Then, three analyaes were used to investigate the questions: whether mean SVI and SGI are centered near normal over the full record; whether average anomaly conditions of both variables changed between 1982–1999 and 2000–2024; and whether a relationship exists between SVI and SGI, including whether it strengthens at a temporal lag.
Bootstrap confidence intervals addressed the first question. By repeatedly resampling monthly observations with replacement and taking the 2.5th and 97.5th percentiles of each bootstrap distribution, 95% confidence intervals were calculated for both means. Both SVI and SGI had mean values close to zero, and both intervals overlapped zero, which is consistent with standardized anomaly indices that are centered near long-term monthly conditions. SVI showed greater spread than SGI, suggesting regional vegetation anomalies fluctuate more strongly over time than groundwater anomalies.
Welch's two-sample t-tests addressed the second question, comparing the two time periods. Mean SVI was significantly higher in 1982–1999 (≈ 0.077) than in 2000–2024 (≈ −0.060), with a p-value well below 0.05. Mean SGI showed no significant difference between periods (p ≈ 0.42), remaining close to zero in both periods. Vegetation anomalies shifted more clearly after 2000, while groundwater anomalies were comparatively stable.
A linear regression addressed the third question, with SGI as the response and SVI as the predictor variables. The same-month model explained virtually no variation in SGI as the R² was near zero, indicating SVI is not a useful predictor of groundwater condition when comparing pairs. However, when considering the delayed response from groundwater, a lag correlation can be performed by repeating the regression after shifting SGI from −12 to +12 months relative to SVI. The strongest association appeared at a positive lag of approximately two months, meaning vegetation anomalies were most closely linked to groundwater anomalies roughly two months later. However even with this lag, the best-lag R² was only about 0.04, indicating a weak though significant lagged relationship rather than a strong predictive one. 
Altogether, the results suggest: mean vegetation conditions have significantly changed between early and later periods than groundwater, and while same-month correlation between the two indices is minimal, vegetation may weakly precede groundwater by about two months. This is physically plausible given the sequential timescales at which vegetation, soil moisture, recharge, and water table depth respond to climate variability. The low R² values, however, make clear that SVI alone is insufficient to explain groundwater dynamics. Furthermore this work averaged the spatial data into a single time series, losing much of the spatial and climatological heterogeneity. Future work should capture local dynamics by aggregating by basin or climate zone and additionally incorporate precipitation, evapotranspiration, and temperautre to better capture the hydroclimatological forcings that drive drought across these systems. 


Write-up of your project and findings go here. Think of this as the text
of your presentation. The length should be roughly 5 minutes when read
out loud. Although pacing varies, a 5-minute speech is roughly 750
words. To use the word count addin, select the text you want to count
the words of (probably this is the Summary section of this document, go
to Addins, and select the `Word count` addin). This addin counts words
using two different algorithms, but the results should be similar and as
long as you’re in the ballpark of 750 words, you’re good! The addin will
ignore code chunks and only count the words in prose.

You can also load your data here and present any analysis results /
plots, but I strongly urge you to keep that to a minimum (maybe only the
most important graphic, if you have one you can choose). And make sure
to hide your code with `echo = FALSE` unless the point you are trying to
make is about the code itself. Your results with proper output and
graphics go in your presentation, this space is for a brief summary of
your project.

## Presentation

Our presentation can be found [here](presentation/presentation.html).

## Data

Include a citation for your data here. See
<http://libraryguides.vu.edu.au/c.php?g=386501&p=4347840> for guidance
on proper citation for datasets. If you got your data off the web, make
sure to note the retrieval date.

## References

List any references here. You should, at a minimum, list your data
source.
