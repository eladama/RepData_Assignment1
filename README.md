# RepData_Assignment1
RepData_Assignment
---
title: "Assignment01"
author: "Adam"
date: "Sunday, April 19, 2015"
output: html_document
---

This is an R Markdown document. made for the first assignement.

Loading and preprocessing the data
----------------------------------

1:Loading the data

```{r}
activities <- read.csv(file="activity.csv", sep="," , head=TRUE)
```

Displaying the summary information from the dataset

```{r}
summary(activities)
```

2: Remark : cleaning data, subset away missing data/ outliner

code:
activitiesb <- subset(activities, activities$steps=NA)

Displaying new summary after processing

code:
summary(activities)



What is mean total number of steps taken per day?
-------------------------------------------------

1:Calculate the total number of steps taken per day

```{r}
nrow(activities)
```

Total is 17568

2: making a histogram

```{r}
hist(activities$steps)
```

