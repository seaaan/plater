---
  title: 'plateR: Tools to Make it Easy to Work with Microtiter Plate-Shaped Data'
  tags:
    - data import
    - R
  authors:
   - name: Sean M Hughes
     orcid: 0000-0002-9409-9405
     affiliation: University of Washington
  date: 25 July 2016
  bibliography: paper.bib
---

# Summary

plateR is an R [@R] package makes it easy to work with data from experiments performed in microtiter plates.

Many scientific instruments (such as plate readers and qPCR machines) produce data in tabular form that mimics a microtiter plate: each cell corresponds to a well as physically laid out on the plate. For experiments like this, it's often easiest to keep records of what was what (control vs. treatment, concentration, sample type, etc.) in a similar plate layout form. 

plateR defines a simple file format for data storage, so it's easy to remember which wells were which, and provides functions to seamlessly convert between that format and a tidy [@tidy] data frame that's optimal for analysis. 

# References