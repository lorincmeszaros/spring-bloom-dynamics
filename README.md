# spring-bloom-dynamics
This repository contains Python 3 scripts for estimating climate change induced uncertainties in phytoplankton spring bloom dynamics. 

The scripts cover:
- data processing
- time series forecasting
- concave regression

Data processing: The data sources are chlorophyll-a concnetrations (in-situ from Rijkswaterstaat, satellite from CMEMS, fused data from https://github.com/fmeulen/DataFusion), air temperature and solar radiation (in-situ from KNMI, climate projections from Euro-CORDEX, synthetic climate prjections from Meszaros et al .(2020)). 

Time series forecasting: using Facebook's Prophet model to forecast chlorophull-a based on the fused historical signal and explanatory variables (air temperature and radiation). 

Concave regression: non-parameetric shape constraint regression to extract cardinal dates (bloom beginning, -peak, -end) of phytoplanton spring blooms.
