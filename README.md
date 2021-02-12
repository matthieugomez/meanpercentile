This package provides a command to decompose the growth of an average wealth in a top wealth percentile into a within term, a displacement term, and a demography term.

The syntax is
```
meanpercentile [varname] using filename [, top(indicatorvariable) replace]
```
where 
- `varname` is the variable to decompose
- `filename` a filepath to save the output as a dataset
- `indicatorvariable` is a dummy variable indicating whether the observation belongs to the top percentile. When not specified, the decomposition is done for the top 100%.

# References

Matthieu Gomez *Decomposing the Growth of Top Wealth Shares*. Working Paper

# Installation

```
net install decompose, from("https://raw.githubusercontent.com/matthieugomez/decomposing_the_growth_of_top_wealth_shares/master/")
```
If you have a version of Stata < 13, you need to install it manually

Click the "Download ZIP" button in the right column to download a zipfile.

Extract it into a folder (e.g. ~/SOMEFOLDER)

Run
```
cap ado uninstall decompose
net install decompose, from("~/SOMEFOLDER")
```