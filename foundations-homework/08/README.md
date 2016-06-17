# Homework8

The dataset I prepared does not hold information for 12 questions, but I still want to work with it. So to make up for the non-asked questions, I decided to sumbit an additional dataset -- so in total it's three. Hope that compromise is okay.  

* Dataset1: **Water** Last year I went to a research trip to Isreal, they are genius at water recycling! That got me interested in the whole area of water pollution/recycling/pricing/share of transfer between countries. Preparing for class Tues evening, I could not find consistent data for all/many countries on these topics. However, the WorldBank had data on Renewable Freshwater Resources and Annual Withdrawl, so I thought that would be a good starting point. As there's the theory of water scarcity being related to outbreak of conflict (most recent example: Syria) that would be a nice correlation to investigate -- yet lacking the conflict-outbreak-data.

* Dataset2:

* Dataset3:

## Useful things:

### DATA

* **positioning of columns**: in Excel, if I calculate sth from column 2 and 3, I would put the result next to it in column 4. Per panda-default, it would be in the last - but there's a command for manipulating: df.insert(index, 'columnname', value)

### PLOTTING

* **Manipulating graphic size** figsize = (width, height)
--> makes the displayed chart bigger. No idea what's the values measurement - px doesn't seem to be the case.
--> play around to find what fits best for your data


## Problematic things:

### DATA

* **NaN, n/a, 0**: For my first data set (the water data) I created in excel a file from three different Worldbank Data tables. Because I already had decided what questions to ask it, I knew that "0" in places where are no data would make my life harder. So I manually deleted the 0 out of the resepctive excel-cells. However, after importing with pd into iPython, some "empty" cells were filled with 0.0000, 0 or NaN instead
--> Takeaway: better to do data cleaning directly in pandas than trying to do that in advance in excel

* **Country-groups**: Worldbank data for all countries often also compromises data for groups of countries (LIC, HIC, Europe, Southeast Asia), that come with the same stucture as normal country data, so it is kind of difficult to get them out of there....

### PLOTTING
