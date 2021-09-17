# ML---Pump-it-up
https://github.com/jayampathiadhikari/ML---Pump-it-up
## Pre-Processing and Feature Engineering

### 1. Removing unnecessary data
The data set contained many data columns which are irrelevant for the functionality of the pupms. First they were identified.

ex: "date_recorded","wpt_name","num_private","recorded_by"

There were several columns which had the same data on different ways. After comparing them using graphs unnecessary columns were identified.

ex: "extraction_type", "extraction_type_group", "extraction_type_class" all these columns contained similar data and by comparing them using graphs best column was selected

This was done to all other similar columns.

### 2. Filling null values

After removing similar columns, dataset was checked for null values.
Several columns had null values and they were categorical columns.
Therefore Null values were filled by the most_frequent values.

### 3. Feature Engineering

The column construction_year had many years varying from 1960s upto 2020s.
So bining was done to reduce the year groups. 
Years were grouped into decades.
Ex: 1960s -> 1, 1970s -> 2, 1980s -> 3
Then "construction_year" column was removed and a new column "year" was added using above decade values


### 4. Encoding

Many of the remaining dataset columns were categorical and they had high cardinality. 
Therfore LabelEncoding was chosed as the encoding method

## Proof
![alt text](https://github.com/jayampathiadhikari/ML---Pump-it-up/blob/main/Screenshot%202021-09-17%20090916.png?raw=true)
![alt text](https://github.com/jayampathiadhikari/ML---Pump-it-up/blob/main/Screenshot%202021-09-17%20090932.png?raw=true)
