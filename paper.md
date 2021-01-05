---
title: 
'Processing spectral induced polarization data in frequency-domain and time-domain using pyBERT'
tags:
  - Python
  - geophysics
  - induced polarization
authors:
  - name: Thomas Günther
    orcid: 0000-0003-0872-7098
    affiliation: 1
affiliations:
 - name: Thomas Günther, Leibniz Institute for Applied Geophysics
   index: 1
date: 13 August 2017

bibliography: paper.bib
---

# Processing spectral induced polarization data in frequency-domain and time-domain using pyBERT

**Summary**

Spectral Induced Polarization (SIP) data can provide valuable insight into subsurface properties such as mineral or clay content. Particularly, the spectral behaviour, measured in either frequency domain (FD) or time domain (TD) gives insight into properties like grain size. For analysing IP field data, a bunch of processing steps is necessary. We present a toolbox with classes for importing data, generating automated plots, filtering, inversion and post-processing, e.g. fitting Cole-Cole models to the results. This will enable non-specialist users to evaluate their data and to obtain meaningful subsurface models.

## Introduction
The method of induced polarization (IP) is an extension of the direct current (DC) method, also known as Electrical Resistivity Tomography (ERT), by measuring not only the voltage amplitude as a result of an injected current, but also its behaviour with time or frequency bearing information on the polarization properties in addition to the resistivity.

The method has been routinely used in the field since the 1970ies, mainly for investigating ore deposits. Metallic materials like ore minerals show considerable polarisation effects that help to ease the interpretation and to distinguish them from other conductive units. Similarly large effects are also known from fault zones bearing graphite zones, or blackshales with either graphite or Pyrite.

As a result of ongoing improvements of measuring instruments, the IP method has also been applied to characterize much less polarizable material like unconsolidated sediments whose polarization is originated from grains and 

## Statement of need
There are several packages for processing ERT data, some of them are open-source. Most codes support IP, but typically only single frequency (FD) or total/integral chargeability (TD) values. To assess the spectral properties of the subsurface, a spectral inversion is needed, which is most robustly done by using regularization along the spatial dimension (time or frequency). This is the first openly available software for processing spectral IP field date.

## Methodology
sdfsdf


```python
import pygimli as pg
print(pg.__version__, pg.__file__)

```

    0+untagged.3579.geafc386 C:\Guenther.T\src\gimli\gimli\pygimli\__init__.py
    


```python
grid = pg.createGrid(4,3)
pg.show(grid)
```




    (<matplotlib.axes._subplots.AxesSubplot at 0x20ec74c8bb0>, None)




![png](output_6_1.png)

