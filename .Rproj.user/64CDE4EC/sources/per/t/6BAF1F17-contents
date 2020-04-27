##Load Package
library('tidyverse')

## Reading the dataset
titanic = read_csv('titanic_train.csv')

## Missing Value
colSums(is.na(titanic))

## Encoding Categorical Variable 
titanic %>%
  mutate(Pclass = factor(Pclass, 
                         levels = c(1:3), 
                         labels = c(1,2,3)))
titanic %>%
  ggplot(aes(x = factor(Pclass), y = Age, fill = factor(Pclass) )) +
  geom_boxplot()
