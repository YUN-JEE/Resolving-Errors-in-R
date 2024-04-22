# How to resolve error you face in R in MAC M1pro 

## "The following object is masked from 'package:base': errorCondition   " 

### Situation 
typed below and got a error message saying " ~ masked ~ errorCondtion"

```
library(Rcmdr)
```
I ignored it and tried to import files to R commander 

But, Whenever I try to open "Documents" directory in R commander, this error message appears below. 
![image](https://github.com/YUN-JEE/RNAseq/assets/164160626/5e5ce72a-b7dc-471a-a3ec-bc5697ce2c74)

or the R commander itself just shuts down automatically 


  ### incomplete Solution
1. Go to [R] 
2. on the upper bar, click [Package & Data] -> [Package Manager] 
3. Check whether there are packages with the same name and are overloaded more than twice. 
      In my case, [Rcmdr], [RcmdrMisc] were loaded twice.
Make sure only one package is loaded for each type

==> This will solve the problem on "Documents" directory. You will be able to access it. 
However, the error message " ~ masked from ~" still appears. 
