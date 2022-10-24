# ccalc  

Command line math expression evaluator - from the original by Steve Hanov: [http://stevehanov.ca/blog/?id=26](http://stevehanov.ca/blog/?id=26)  
The source code that I started with was available on 20 June 2019 at: [http://stevehanov.ca/blog/calc.c](http://stevehanov.ca/blog/calc.c)   
This is a simple command line calculator to save you the clicks or keystrokes required by many common options.  I think it is the best for simple, [rough](https://www.explainxkcd.com/wiki/index.php/2205:_Types_of_Approximation) calculations and it works well for my day-to-day workflow in a Windows environment.  

For example;  

```
C:\>ccalc 100/(412117/78221)  
18.980290  
  
C:\>ccalc 0x961
2401.000000
  
C:\>ccalc (3500000 * .03)  
105000.00  
  
``` 

In a Linux environment, ```bc``` is already available for analygous command line math:  
```terminal
user@host:~$ bc -l <<< "scale=2 ; 100/(412117/78221)"
19.01
```
(*Note the [rounding difference](https://www.explainxkcd.com/wiki/index.php/2205:_Types_of_Approximation).  If you are looking for precise results, use tooling purpose built for your needs.*)  
