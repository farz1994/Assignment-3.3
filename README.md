Test whether two vectors are exactly equal (element by element). vec1 = c(rownames(mtcars[1:15,])) vec2 = c(rownames(mtcars[11:25,]))
> vec1 = c(rownames(mtcars[1:15,]))
> vec2 = c(rownames(mtcars[11:25,]))
> identical(vec1, vec2)
[1] FALSE

2. Sort the character vector in ascending order and descending order. vec1 = c(rownames(mtcars[1:15,])) vec2 = c(rownames(mtcars[11:25,]))
# In ascending order
> sort(vec1, vec2, decreasing = FALSE)
 [1] "Cadillac Fleetwood" "Datsun 710"         "Duster 360"         "Hornet 4 Drive"    
 [5] "Hornet Sportabout"  "Mazda RX4"          "Mazda RX4 Wag"      "Merc 230"          
 [9] "Merc 240D"          "Merc 280"           "Merc 280C"          "Merc 450SE"        
[13] "Merc 450SL"         "Merc 450SLC"        "Valiant" 
# In descending order
> sort(vec1, vec2, decreasing = TRUE)
 [1] "Valiant"            "Merc 450SLC"        "Merc 450SL"         "Merc 450SE"        
 [5] "Merc 280C"          "Merc 280"           "Merc 240D"          "Merc 230"          
 [9] "Mazda RX4 Wag"      "Mazda RX4"          "Hornet Sportabout"  "Hornet 4 Drive"    
[13] "Duster 360"         "Datsun 710"         "Cadillac Fleetwood"

3. What is the major difference between str() and paste() show an example.
str() : Only one line of each basic structure is displayed, used to display the internal structure of an R object.
paste() : Complete list is shown as the result, used to concatenate 2 or more Strings.

Example :
> str(vec1, vec2)
 chr [1:15] "Mazda RX4" "Mazda RX4 Wag" "Datsun 710" "Hornet 4 Drive" ...
> paste(vec1, vec2)
 [1] "Mazda RX4 Merc 280C"                  "Mazda RX4 Wag Merc 450SE"            
 [3] "Datsun 710 Merc 450SL"                "Hornet 4 Drive Merc 450SLC"          
 [5] "Hornet Sportabout Cadillac Fleetwood" "Valiant Lincoln Continental"         
 [7] "Duster 360 Chrysler Imperial"         "Merc 240D Fiat 128"                  
 [9] "Merc 230 Honda Civic"                 "Merc 280 Toyota Corolla"             
[11] "Merc 280C Toyota Corona"              "Merc 450SE Dodge Challenger"         
[13] "Merc 450SL AMC Javelin"               "Merc 450SLC Camaro Z28"              
[15] "Cadillac Fleetwood Pontiac Firebird" 



4. Introduce a separator when concatenating the strings.
> paste(vec1, vec2, sep = " ")
 [1] "Mazda RX4 Merc 280C"                  "Mazda RX4 Wag Merc 450SE"            
 [3] "Datsun 710 Merc 450SL"                "Hornet 4 Drive Merc 450SLC"          
 [5] "Hornet Sportabout Cadillac Fleetwood" "Valiant Lincoln Continental"         
 [7] "Duster 360 Chrysler Imperial"         "Merc 240D Fiat 128"                  
 [9] "Merc 230 Honda Civic"                 "Merc 280 Toyota Corolla"             
[11] "Merc 280C Toyota Corona"              "Merc 450SE Dodge Challenger"         
[13] "Merc 450SL AMC Javelin"               "Merc 450SLC Camaro Z28"              
[15] "Cadillac Fleetwood Pontiac Firebird" 
