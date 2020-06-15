---
title: "Diss Power"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```
Create data set with phq-9, gender, pre and post scores
```{r}
phq9_pre = rnorm(100, 6, 2)
phq9_post = rnorm(100, 4, 1)
gender_samp = c(1,0)
gender = sample(gender_samp, 100, replace = TRUE)
dat_qlik = data.frame(phq9_pre, phq9_post, gender)
write.csv(dat_qlik, "dat_qlik.csv", row.names = FALSE)

```



 

