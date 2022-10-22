spol <- c('muško', 'žensko', 'muško', 'žensko', 'muško')
spol
spol_f <- factor(spol)
spol_f
#spol_f[1]<spol_f[2]


#temps <- factor(c('visoka', 'visoka', 'niska', 'srednja', 'srednja', 'srednja'))
#temps

#levels(temps) <- c('niska', 'srednja', 'visoka')
#temps
#levels(temps[1]) < levels(temps[2])

t <- (c('visoka', 'visoka', 'niska', 'srednja', 'srednja', 'srednja'))
l <- c('niska', 'srednja', 'visoka')
temp <- factor(t, levels = l, order = T)
temp

#install.packages("gapminder")
#install.packages("dplyr")
library('gapminder')
library('dplyr')
gapminder %>% filter(year==1993, country == 'Croatia')

# pipes
hrvatska <- gapminder%>%
  arrange(desc(year))%>%
  filter(country == 'Croatia')
# or
#hrvatska <- gapminder %>% arrange(desc(year)) %>% filter(country == 'Croatia')
hrvatska

# if we modify variable name, a new column is added at the end
gapminder %>% mutate (pop2 = pop / 100000)

# Task 1
hr <- gapminder %>% filter(country == 'Croatia') %>% mutate (populacija = pop / 1000000)
hr

# Task 2
year_populacija = cbind(hr[,3], hr[,7])

# Task 3
year_populacija %>% arrange (desc(year))