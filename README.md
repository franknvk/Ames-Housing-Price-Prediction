## Problem Statement
Popularity in house flipping has become a lucrative business since HGTV's Fixer Upper and Flip or Flop became popular. Average home flipping profits average to around $65000 but return on investment has been steady declining year over year due to increased median home prices and rising construction costs. To help house flippers, the simpliest and most effective atrributes of a home are more important than ever. In this Ames housing data, we aim to find the best neighborhood for buying cheap and selling high. Once we find the best area, we will correlate the best features in that area to quickly and ecomically increase value of the home overall.   

source: https://www.fool.com/research/house-flipping-statistics/

## Audience
Interested parties in house flipping investments.

## Data Dictionary 
|Feature|Type|Dataset|Description|
|---|---|---|---|
|id|int|1a.data_cleaning(train)|observation number|
|pid|int|1a.data_cleaning(train)|parcel identification number - can be used with city web site for parcel review|
|mssubclass|int|1a.data_cleaning(train)|Identifies the type of dwelling involved in the sale|
|mszoning|object|1a.data_cleaning(train)|Identifies the general zoning classification of the sale|
|lotfrontage|float|1a.data_cleaning(train)|Linear feet of street connected to property|
|lotarea|int|1a.data_cleaning(train)|Lot size in square feet| 
|street|object|1a.data_cleaning(train)|Type of road access to property|
|lotshape|object|1a.data_cleaning(train)|General shape of property|
|landcontour|object|1a.data_cleaning(train)|Flatness of the property|
|utilities|object|1a.data_cleaning(train)|Type of utilities available|
|lotconfig|object|1a.data_cleaning(train)|Lot configuration|
|landslope|object|1a.data_cleaning(train)|Slope of property|
|neighborhood|object|1a.data_cleaning(train)|Physical locations within Ames city limits|
|condition1|object|1a.data_cleaning(train)|Proximity to various conditions|
|condition2|object|1a.data_cleaning(train)|Proximity to various conditions -if more than one is present|
|bldgtype|object|1a.data_cleaning(train)|Type of dwelling|
|housestyle|object|1a.data_cleaning(train)|Style of dwelling|
|overallqual|int|1a.data_cleaning(train)|Rates the overall material and finish of the house|
|overallcond|int|1a.data_cleaning(train)|Rates the overall condition of the house| 
|yearbuilt|int|1a.data_cleaning(train)|Original construction date|
|yearremod_add|int|1a.data_cleaning(train)|Remodel date-same as construction date if no remodeling or additions|
|roofstyle|object|1a.data_cleaning(train)|Type of roof|
|roofmatl|object|1a.data_cleaning(train)|Roof material|
|exterior1st|object|1a.data_cleaning(train)|Exterior covering on house|
|exterior2nd|object|1a.data_cleaning(train)|Exterior covering on house-if more than one material|
|masvnrtype|object|1a.data_cleaning(train)|Masonry veneer type| 
|masvnrarea|float|1a.data_cleaning(train)|Masonry veneer area in square feet|
|exterqual|object|1a.data_cleaning(train)|Evaluates the quality of the material on the exterior|
|extercond|object|1a.data_cleaning(train)|Evaluates the present condition of the material on the exterior|
|foundation|object|1a.data_cleaning(train)|Type of foundation|
|bsmtqual|object|1a.data_cleaning(train)|Evaluates the height of the basement|
|bsmtcond|object|1a.data_cleaning(train)|Evaluates the general condition of the basement|
|bsmtexposure|object|1a.data_cleaning(train)|Refers to walkout or garden level walls|
|bsmtfintype1|object|1a.data_cleaning(train)|Rating of basement finished area|
|bsmtfinsf1|float|1a.data_cleaning(train)|Type 1 finished square feet|
|bsmtfintype2|object|1a.data_cleaning(train)|Rating of basement finished area-if multiple types|
|bsmtfinsf2|float|1a.data_cleaning(train)|Type 2 finished square feet|
|bsmtunfsf|float|1a.data_cleaning(train)|Unfinished square feet of basement area|
|totalbsmtsf|float|1a.data_cleaning(train)|Total square feet of basement area|
|heating|object|1a.data_cleaning(train)|Type of heating|
|heatingqc|object|1a.data_cleaning(train)|Heating quality and condition|
|centralair|object|1a.data_cleaning(train)|Central air conditioning|
|electrical|object|1a.data_cleaning(train)|Electrical system| 
|1stflrsf|int|1a.data_cleaning(train)|First Floor square feet|
|2ndflrsf |int|1a.data_cleaning(train)|Second floor square feet|
|lowqualfinsf|int|1a.data_cleaning(train)|Low quality finished square feet-all floors|
|grlivarea|int|1a.data_cleaning(train)|Above grade (ground) living area square feet|
|bsmtfullbath|float|1a.data_cleaning(train)|Basement full bathrooms|
|bsmthalfbath |float|1a.data_cleaning(train)|Basement half bathrooms|
|fullbath|int|1a.data_cleaning(train)|Full bathrooms above grade|
|halfbath|int|1a.data_cleaning(train)|Half baths above grade|
|bedroomabvgr|int|1a.data_cleaning(train)|Total rooms above ground|
|kitchenabvgr|int|1a.data_cleaning(train)|Kitchens above grade|
|kitchenqual|object|1a.data_cleaning(train)|Kitchen quality|
|totrmsabvgrd|int|1a.data_cleaning(train)|Total rooms above grade (does not include bathrooms)|
|functional|object|1a.data_cleaning(train)|Home functionality|
|fireplaces |int|1a.data_cleaning(train)|Number of fireplaces|
|garagetype |object|1a.data_cleaning(train)|Garage location|
|garageyrblt|float|1a.data_cleaning(train)|Year garage was built|
|garagefinish|object|1a.data_cleaning(train)|Interior finish of the garage|
|garagecars|float|1a.data_cleaning(train)|Size of garage in car capacity|
|garagearea |float|1a.data_cleaning(train)|Size of garage in square feet|
|garagequal|object|1a.data_cleaning(train)|Garage quality|
|garagecond|object|1a.data_cleaning(train)|Garage condition|
|paveddrive|object|1a.data_cleaning(train)|Paved driveway|
|wooddecksf|int|1a.data_cleaning(train)|Wood deck area in square feet|
|openporchsf|int|1a.data_cleaning(train)|Open porch area in square feet|
|enclosedporch|int|1a.data_cleaning(train)|Enclosed porch area in square feet|
|3ssnporch|int|1a.data_cleaning(train)|Three season porch area in square feet|
|screenporch|int|1a.data_cleaning(train)|Screen porch area in square feet|
|poolarea|int|1a.data_cleaning(train)|Pool area in square feet|
|miscfeature|object|1a.data_cleaning(train)|Miscellaneous feature not covered in other categories|
|miscval|int|1a.data_cleaning(train)|Value of miscellaneous feature|
|mosold|int|1a.data_cleaning(train)|Month Sold|
|yrsold|int|1a.data_cleaning(train)|Year Sold|
|saletype|object|1a.data_cleaning(train)|Type of sale|
|saleprice|int|1a.data_cleaning(train)|Sale price in USD|
|has_garage|int|1a.data_cleaning(train)|1-has garage, 0- does not have garage|
|has_pool| int|1a.data_cleaning(train)|1-has poole, 0- does not have pool|
|has_basement| int|1a.data_cleaning(train)|1-has basement, 0- does not have basement|
|has_fence|int|1a.data_cleaning(train)|1-has fence, 0- does not have fence|
|has_alley|int|1a.data_cleaning(train)|1-has alley, 0- does not have alley|

## Summary of Analysis

Intial Processing: Read in Ames housing data and inspected data set. The target data was not normally distributed but not so much that it effected modeling. From there, I split the data into training and testing datasets. I then split those into type specific dataframes. From each type-dataframe, I checked for null and filled accordingly to the data dictionary. I then imputed any other values needed, usally only filling 1-2 values. I then scaled the numeric data, encoded the ordinal data based on a dicionary, and dummied the nominal data. Afterwards, I combined all type dataframes back together, with the conneced ID, and exported the train and test dataframes in order to use in EDA, visualization, and modeling. 

EDA + Visualization: Kaggle Submission: I explored different correlated variables in a heat map. From there, we saw a lot of multicolinear variables and decided to move forward with a VIF test to drop variables that were too similar. From there, I checked linear relationships with the remaining variables. I did decided to go wih two different data sets to compare models. First was the VIF condensed dataframe and second was the top correlatted variables from the VIF dataframe. 

Ames Presentation: For this project, I found the highest mean sold house neighborhood and condensed my dataframe from that specific area. From there, linear relationships were established from the predictor variables. Picking the highest and lowest correlated variables, I created a new dataframe to use in the modeling.

Modeling: Kaggle: I compared Linear Regression and Gridsearch CV with Lasso and Ridge. I check cross val scores and r2 scores to compare validity of the model. Overall, the linear model did the worst and Lasso did the best using the VIF model. The correlated variable dataframe was similar but not as good as the VIF. In the lasso model. the mean square error was better than the baseline and the R2 scores for the test and the train were close together showing the model was not overfit to the training data. 

## Conclusions and Reccomendations

**Conclusions:**
If looking to flip a home as an invest, look to purchase in the Ridge Brooke area. Northridge Heights has potential that can be further examined based on range of home prices.Total living area and lot size have large factor in resale value though expensive to change. External house material has a large impact: use masonry siding for maximum returns Adding a garage and fireplace and converting a covered porch to a screen porch will increase value.

**Research**
Refine model to work over different neighborhoods. Check the proximity to important features like a university or
major hospital, and see how tha changes neighborhood selection. Research HOA regulations to check agains additional costs and renovation regulations.