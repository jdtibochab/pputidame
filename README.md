ME-model of *P. putida* KT2440 (*i*Ppu1676-ME)
=============================================

This repository contains all the information and building scripts required to construct a ME-model for *P. putida* KT2440, *i*Ppu1676-ME using
[coralME](https://github.com/jdtibochab/coralME).


Install locally
---------------
1. Clone repository
2. run ```pip install -r requirements.txt```

Install using Docker
--------------------
1. Clone repository
2. ``docker build --file "./Dockerfile-Python3.10" . -t "pputidame"``
3. ``docker run --detach -p 10000:8888 -v USER/PATH/TO/pputidame/:/opt/notebooks/ pputidame`` 
4. In your browser, go to ``localhost:10000``

Understanding the layout of this repository
-------------------------------------------
Jupyter Notebooks contain the following analyses:

0. Reconstruction and constraining of the ME-model
1. Omics overview and analysis
2. Comparison of model predictions and omics
3. Final visualization of the comparison of model predictions and omics
4. Allocation observed in the omics data
5. Flux Variability Analysis of M- and ME-models
6. Analysis of intracellular phenotype (comparison with MFA)
