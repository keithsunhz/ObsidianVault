# R Studio Cheatsheet

## Importing data

- attach(nameofdataset) : makes working with current dataset so much easier. this will put the data into R memory so you can use the variables without typing "nameofdataset$variable"
	- detach(nameofdataset) is to detach data

- as.factor: this changes character variable to factor
	- e.g. LungCapData$ Smoke <- as.factor(LungCapData$Smoke)


- levels(): this checks the type of variable. cat vs num

## Plots

- barplot() - bar graph
- pie() - piechart
- boxplot() - boxplot
- hist() - histogram

## Hypothesis Testing

### Continuous testing
- t.test() - comparing means of 2 pop
- wilcox.test() - comparing median of 2 pop
- aov() - ANOVA used to compare means of 2 or more pop
	- TukeyHSD() - used to see which pop  differs from others
	- https://youtu.be/lpdFr5SZR0Q
	- kruskal.test() - nonparametric method of ANOVA

### Categorical testing
- table() - creates 2x2 table
- prop.table() - gives proportion (%) of a table

- chisq.test()
- fisher.test()
- epi.2by2() - this uses EpiR package. computes RR and OR