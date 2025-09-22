# IDS 
c <- 3
a <- 32
library(tidyverse)
test <- tibble(
 clm1 = c("one", "two", "three", a),
 numerical = c(1, 2, 3, a)
)
p1 <- ggplot(data = test,
             mapping = aes(x = clm1,
             y = numerical)
             )+
   geom_col() +
   scale_fill_identity()
p1

