Pitch
========================================================
author: Srindhi Sridhar
date: 28/07/2020
autosize: true

Overview
========================================================

- ABCD grade calulcator will quantify the overall performance of indiviual assessment and give the grade based on the weight of each assessment.
- The weightage is: 
- 1.1st Semester marks-20% 
- 2.2nd Semester Marks-20% 
- 3.Final Exam Marks-40% 
- 4.Practical Exam Marks-10%
- 5.Sports Marks-5% 
- 6.Community Development marks-5%
Code
========================================================
Calculations and rounding performed by the a simple code. This is the calculation for the final grade of the year, using weightage


```r
number = round((semi1*.2)+(semi2*.2)+(input$final*.4)+(pract*.1)+(sport*.05)+(commd*.05))
```
Plot
========================================================
The following code is used to plot the weight plot of each mark received


```r
dat<-matrix(c(33, 17, 10 ,20 , 20), ncol = 1, nrow = 5)
    barplot(dat, horiz = TRUE, yaxt="n", xlab = "number", main="Your Performance", col=c("red", "blue", "yellow", "grey", "black"))
    lines(x=c(21, 21), y=c(0,1.2), col="White", lwd=4)
```

![plot of chunk unnamed-chunk-2](Pitch-figure/unnamed-chunk-2-1.png)
Thank You
============================================================
This is a basic representation of the Shiny app and Presentation that can be done as part of the 'Developing Data Products' Course of John Hopkins Data Science Specialisation
