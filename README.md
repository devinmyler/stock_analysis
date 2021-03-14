# An Analysis of Stock Tickers and Refactoring VBA Code
## Overview of Project
The purpose of the analysis was to help a friend see and choose stocks from a small dataset. The data was limited to twelve stocks and their movements along a two year period. 
Although our analysis was only based on 12 stocks, the code we wrote to analyse the return and the total volume of those stocks could be utilized to view the movement of the stockmarket as a whole. In order for that to be possible, the code would have to be refactored to run faster.
By creating new output arrays and using for loops more efficiently, we can reduce the number of times the information must be cycled over in order to obtain the desired information.
## Results
### Initial Code
Before the new arrays were utilized, the code ran decently quickly. ![VBA_Challenge_2017_initial](https://user-images.githubusercontent.com/78869891/111086978-8b120500-84f5-11eb-8d95-6849d1a27019.png)
![VBA_Challenge_2018_initial](https://user-images.githubusercontent.com/78869891/111086980-8cdbc880-84f5-11eb-8218-38ecb0b16f0c.png)
As we can see here, the code runs over the 12 stocks and returns the information in about half a second. It doesn't seem problematic at the moment. However, if run on a less powerfyl machine, or used to look over more than twelve stocks, or gathering information from more than two years, this number could be much, much higher.
### Refactored code
Once the new arrays are listed, the code runs much faster. Nearly ten times faster! ![VBA_CHallenge_2017_refactored](https://user-images.githubusercontent.com/78869891/111087082-f78d0400-84f5-11eb-8489-452f35b82c9d.png)
![VBA_Challenge_2018_refactored](https://user-images.githubusercontent.com/78869891/111087085-f8be3100-84f5-11eb-988b-b7bf3c81300d.png)
These results show promise for expanding our analysis in the future, whether that means adding more stocks or more years, the new code is able to handle the traffic much better than the initial code.
## Summary
As you can see, the advantage to refactoring code show themselves quite clearly in run speed. If using this code repeatedly, or sharing it with others, the amount of time the refactored code saves would become very large. However, if the code was being used sparsely or by few, the time it takes to refactor working code could potentially outweigh the amount of time saved by the refactored code; and if it takes longer to write than the time it would save, what's the point?
The main takeaway would be to write the code efficiently in the first place. Then you get 'refactored' speeds, without the time it takes to refactor the code. 
