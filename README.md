# Berkeley ML-AI Course Practical Application 2 Assignment

## This describes the analysis conducted on the available data and conclusions about the 
## factors that have the most influence on the price of a used car.

## Since the available data did not have the original sales price of the vehicle when it was new,
## this analyis does not comment on how well a vehicle maintains its value over time.
## The analysis focuses on what characteristics of used vehicles are most associated with the vehicle price.

## A. Data Adjustments
### 1. There were extensive adjustments to the available data to esure the results would be useful.
### The adjustments assume the client is operating a typical used car dealership which sells cars and
### non-commercial trucks.
### The primary adjustments were:
#### 1. Dropped parts of the dataset with significant missing information or data that was not useful
#### or lacked clarity (e.g., references to the vehicle fuel as "other")
#### 2. Some types of information were not useful for this project.  These include: i) the VIN which has no
#### apparent relationship to the vehicle price; ii) very high-mileage vehicles (odometer reading greater than
#### 150,000 miles); iii) vehicles that would presumably not be sold by the client (buses and motorcycles); and
#### iv) information about the vehicle title status (assuming that buyer interest in vehicles without a clean
#### title would be very low).
#### 3. Information about vehicle models was highly challenging to take into account due to inconsistencies.
#### The time alloted for this project did not allow model to be used.  Manufacturer information is available.

## B. Findings
### 1. Some factors for which data are available did not show any substantive influence on vehicle price.
### This included the i) state from which the vehicle came, even after looking at cars from the 20 coldest states 
### vs. other states; ii) the color of the car's paint; iii) whether the transmission was manual or automatic; and
### iv) the number of cylinders (though there were some small indications that 6-cylinder vehicles tend to command
### a higher price).
### 2. The strongest influences on vehicle price were the year of the vehicle's manufacture, the odometer reading,
### whether the vehicle was a truck, whether the vehicle was 4-wheel drive, and whether the vehicle was from a 
### Korean manufacturer.  More specifically:
#### Year -- For vehicles from 2010 and earlier, differences in the year had little impact on the price.  
#### However, the rate at which prices increased for vehicles newer than 2010 grew for new model years (see figure).

<img width="640" height="480" alt="price_by_year_nonlinear_fit" src="https://github.com/user-attachments/assets/ff789c70-75bb-4011-8ee3-cac3e70b9d44" />

#### Odometer -- The higher the odometer reading, the more likely the vehicle's value will be lower.
#### Trucks -- Trucks generally commanded higher prices than other vehicles.  It is worth noting that vehicles using  
#### diesel fuel tended to command higher prices but this is probably because trucks are more likely to use diesel.
#### 4-wheel drive -- 4-wheel drive vehicles commanded higher prices relative to vehicles with front-wheel or
#### rear-wheel drive.  It is worth noting that the data show rear-wheel drive is associated much more with older
#### vehicles which contributes to the lower prices associated with rear-wheel drive vehicles.
#### In addition, the vast majority of sedans have front-wheel drive which tend to 
#### increase the price of sedans though not by a significant amount.
#### Korea -- Korean vehicles had notably lower prices than vehicles from non-Korean 
#### manufacturers.  This may be related to the age of Korean vehicles (average year is 2013).
### 3. To give an idea of how some of the key factors noted above influence the price
### of a car, here are price predictions based on the analysis:
#### Year 2008, no 4-wheel drive, not a truck, 70,000 miles $11,368
#### Year 2020, no 4-wheel drive, not a truck, 70,000 miles $36,962
#### Year 2016, 4-wheel drive, truck, 30,000 miles $23,506
#### Year 2018, 4-wheel drive, not a truck, 40,000 miles $29,502

## C. Overall Conclusions
### Year of manufacture has the greatest influence on vehicle price, with
### particularly strong positive influence for the most recent years.
### Other factors such as whether the vehicle is a truck and the odometer reading
### are important though less so than year.
