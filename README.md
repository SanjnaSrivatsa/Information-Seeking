# Information-Seeking

-----
-------
Files
-------
-----

	
The focal dataset used is 
-------------
* Libraries.csv
--------------	
	This file contains demographic details of all seven libraries in Howard County, Maryland. These details entail name of the library,a unique 
	identification number and segmented address specifics.
 
		( tuple entries for all columns are unique).

Reference: 
Howard County,Maryland. (updated 2014, November 14). Libraries [Data file].
Retrieved from https://data.howardcountymd.gov/geoserver/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=general:Libraries&outputFormat=csv	
	
	

The other datasets used to aid in analysis are:

* Schools_Private.csv

	This file contains demographic details of all twenty three Private Schools in Howard County, Maryland. These details entail name of the school,a unique 
	identification number and segmented address specifics.
 
		( tuple entries for columns 'FID' 'name' and 'address' are unique,
		  tuple entries for columns 'Zipcode' and 'city' have redundancy).

Reference: 
Howard County,Maryland. (updated 2014, November 14). Schools_Private [Data file].
Retrieved from https://data.howardcountymd.gov/geoserver/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=general:Schools_Private&outputFormat=csv

* Elementary_School_District.csv

	This file contains demographic details of all fifty one (Private and Public) Schools in Howard County, Maryland. These details entail name of the 
	elementary school(given as 'ES_HOME'),a unique identification number for the various districts and segmented address specifics( street address 1, street address 2 
	and the geographic coordinates of the exact location of the school given as 'geom').
 
		( tuple entries for columns 'FID' and 'geom' are unique,
		  tuple entries for columns 'ES_HOME', 'STREET1' and 'STREET2' have redundancy).

Reference: 
Howard County,Maryland. (updated 2014, November 14). Elementary_School_District [Data file].
Retrieved from https://data.howardcountymd.gov/geoserver/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=general:Elementary_School_Districts&outputFormat=csv




The dataset obtained on joining 'Private_Schools' and 'Libraries' is 'Howard_County_Libraries_Schools'

The steps taken in building this dataset and other details are documneted in a word file named 'Processing Documentation'

 
* Howard_County_Libraries_Schools.csv

	This file contains demographic details of all Schools and Libraries in Howard County, Maryland . These details entail name of the school,a unique 
	identification number and segmented address specifics.
 
		( tuple entries for columns 'FID' 'name' and 'address' are unique,
		  tuple entries for columns 'Zipcode' and 'city' have redundancy).


Reference: 
Sanjna Srivtsa. ( 2015, October 27). Howard_County_Libraries_Schools [Data file].
Available from https://github.com/SanjnaSrivatsa/Information-Seeking

License:

This work is licensed under the Creative Commons Attribution 4.0 International License. To view a copy of this license, 
visit http://creativecommons.org/licenses/by/4.0/.

	
		
	
 	

-----------
----------
Data format
-----------
-----------

   
The data is formatted one entry per line as follows:
   
	

* Libraries.csv
		FID		Name		Address		City		Zipcode		geom
	
	

* Schools_Private.csv
		FID		Name		Address		City		Zipcode 
	
* Elementary_School_District.csv
		FID		ES_HOME		STREET1		STREET2		geom

-----------
-------
Research Question
-----------

-------

On combining these two datasets the new dataset will help us analyze if schools (only private in this context as public schools cannot decide their 
location independently) consider the presence of libraries in the vicinity while choosing a location for the campus building. We have the data required 
to make an analysis to solve this question. The dataset is reorganised to give us a view of how many schools are situated near a library ,so we can infer if 
private schools consider location of nearby libraries while choosing their campus location. It is important to note that the reason only private schools are considered 
is that public schools do not have a say in where they are located and that is a county level decision and the school independently cannot choose a location
close to the library. However if we wish to take this project forward or dig deeper we can consider a dataset for public schools and determine only weather the county
has already been considering the location of libraries while deciding on a location for a school and if the private schools should follow the same trend. 
For now ,we will consider only private schools and libary locations for our current scope of the research question.









