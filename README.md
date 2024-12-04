ME-model of *P.putida KT2440* (*i*Ppu1676-ME)
=============================================

This repository contains all the information and building scripts required to construct a ME-model for *P. putida KT2440*, *i*Ppu1676-ME using
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
Jupyter Notebooks are ordered here in logical order, where 

0. include reconstruction and constraining of the ME-model
1. include omics overview and analysis
2. include comparison of model predictions and omics
3. include the final visualization of the comparison
4. include the allocation observed in the omics data
