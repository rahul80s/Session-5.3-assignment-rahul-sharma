# Session-5.3-assignment-rahul-sharma
Acagild session 5.3 assignment

1. Test whether two vectors are exactly equal (element by element).

vec1 = c(rownames(mtcars[1:15,]))

vec2 = c(rownames(mtcars[11:25,]))

Ans 1 ->

identical(vec1, vec2)


2. Sort the character vector in ascending order and descending order.

vec1 = c(rownames(mtcars[1:15,]))

vec2 = c(rownames(mtcars[11:25,]))

Ans 2  ->

sort(vec1)

sort(vec1, decreasing = true)


3. What is the major difference between str() and paste() show an example.

Ans 3 -> 

The difference between str() and paste(): zero length arguments like NULL and character(0) are silently removed by str c().  

Also, str() will show the output in one line whereas paste() will show the output in full display. Below is the example:

vec1 = c(rownames(mtcars[1:15,]))

str(vec1)
 
 chr [1:15] "Mazda RX4" "Mazda RX4 Wag" "Datsun 710" ...

paste(vec1)

 [1] "Mazda RX4"          "Mazda RX4 Wag"     
 [3] "Datsun 710"         "Hornet 4 Drive"    
 [5] "Hornet Sportabout"  "Valiant"           
 [7] "Duster 360"         "Merc 240D"         
 [9] "Merc 230"           "Merc 280"          
[11] "Merc 280C"          "Merc 450SE"        
[13] "Merc 450SL"         "Merc 450SLC"       
[15] "Cadillac Fleetwood"


4. Introduce a separator when concatenating the strings.

Ans 4 ->

If we want to change the default separator, we can specify the argument sep:

stri_c("I", "live", "in", "New", "Delhi", sep = "_")

## [1] "I_live_in_New_Delhi"
