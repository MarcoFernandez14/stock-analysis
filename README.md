# stock-analysis

## Overview of Project

### Background
I initially prepared VBA analysis for Steve to help him to evaluate his parent's investments in stocks. The analysis captures a set of 12 stocks and calculates the Total Daily Volume and Return.   
Steve now wants to expand the dataset to include the entire stock market over the last few years. Although the code works well for a dozen stocks, it might not work as well for thousands of stocks. And if it does, it may take a long time to execute.

### Purpose
The ourpoise is to edit or **refactor** the code to loop through all the data one time in order to collect the same information than in the original analysis but more efficiently. The efficeincy of the code will be evaluated according to the time it takes to run.

## Results
### Code refactoring.
The main change to the code is the addition of 3 new arrays: 
* tickerVolumes(12)
* tickerStartingPrices(12)
* tickerEndingPrices(12)

The 3 arrays store performance data for each stock when a for loop runs analysis on them. The tickers array that I created in the original establishes a ticker symbol that can be called on for each stock.

The 3 arrays can be match to ticker array using the variable **tickerIndex**.

### Code running time
The running time decreased from 0.78125 seconds to 0.1796875 seconds (-77%) for 2017 and 0.8515625 to 0.203125 (-76%) for 2018.
* Original 2017

![Original 2017](https://github.com/MarcoFernandez14/stock-analysis/blob/main/Resources/Original%202017.png)
* Refactored 2017

![Refactored 2017](https://github.com/MarcoFernandez14/stock-analysis/blob/main/Resources/VBA_Challenge_2017.png)
* Original 2018

![Original 2018](https://github.com/MarcoFernandez14/stock-analysis/blob/main/Resources/Original%202018.png)
* Refactored 2018

![Refactored 2018](https://github.com/MarcoFernandez14/stock-analysis/blob/main/Resources/VBA_Challenge_2018.png)

## Summary
### There is a detailed statement on the advantages and disadvantages of refactoring code in general.
The main advantage of refactoring code is that it makes it more efficient. The running time reduction can be used to mesure efficiency.
To have an efficient code means that it can handle more data (or the same data using less resources).
The main disadvante is that we can break the code while refactoring. It is impotant to save the progress and check the output regularly.
### There is a detailed statement on the advantages and disadvantages of the original and refactored VBA script.
I think that the only advantage of the original code is that it is easier to read and understand. The refactored code advantages and disadvantages are described in the paragraph above.



