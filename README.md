## assignment 1

Code:

x <- 1:1000 y <- 1:1000 east <- sample(x, size = 75, replace = TRUE) north <- sample(y, size = 75, replace = TRUE) symbols(east, north, squares = rep(.75,10), inches = FALSE) Error in symbols(east, north, squares = rep(0.75, 10), inches = FALSE) : x/y/parameter length mismatch

symbols(east, north, squares = rep(75,10), inches = FALSE) Error in symbols(east, north, squares = rep(75, 10), inches = FALSE) : x/y/parameter length mismatch symbols(east, north, squares = rep(.75,75), inches = FALSE) symbols(sample(x, 40, replace = TRUE),

sample(y, 40, replace = TRUE), 
circles = rep(10,40), 
inches = FALSE,
fg = "green1",
bg = "beige",
add = TRUE)
symbols(sample(x, 12, replace = TRUE),

sample(y, 12, replace = TRUE),
circles = rep(20,12),
inches = FALSE,
fg = "green4",
bg = "beige",
add = TRUE)
dwellings <- cbind.data.frame(id = 1:50, east, north) Error in data.frame(..., check.names = FALSE) : arguments imply differing number of rows: 50, 75 dwellings <- cbind.data.frame(id = 1:75, east, north) locs <- sample(1:10, 7, replace = FALSE) text(x = dwellings[locs, ]$east,

y = dwellings[locs, ]$north + 50, labels = dwellings[locs, ]$id) xspline(x = dwellings[locs, 2], # Easterly coordinate

y = dwellings[locs, 3], # Northernly coordinate
shape = -1,
lty = 2)
title(main="Challenge Question")

I set the X and Y value to 1000 as the minimum. I randomy placed 50 dwelling units, 40 small circle and 12 large trees on the graph. Finally I randomly selected 7 homes and titled the plot.

![graph of challenge question](challenge question.PNG)


# assignment 2

