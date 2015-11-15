# Microsoft-Rugby-Machine-Learning
HackPrinceton Fall 2015 November 13-15
By: Adam Li, Andy Tsai, Richard Chen

01: Download Rugby Dataset from http://rfuchallenge.azurewebsites.net/
The game statistics and timing are:
	1st half: 19:31:34 - 20:17:36
	2nd half: 20:30:34 - 21:20:26
	Field Dimensions: 100m x 68m

01 (Optional) With Azure:
1. portal.azure.com
2. create new 
	- select framework
3. mkdir on desktop and git init
4. deployment credentials username and pw 
5. continuous deployment - git local repo
6. properties - copy git clone the git url
7. git remote add azure <gitcloneurl>

02: Preprocess Data:
Use hackPrinceton_2.7ipynb, or generateJSON.py to preprocess and filter data and reject outliers using gaussian filter. Creates JSON data in the preprocessed_averaged folder. (preprocessed has all the data w/o averaging)

03: Database Connection:
Use mongopreprocess_step2.ipynb to insert JSON data into a mongoDB named 'hackprinceton'. This will have all the data for efficient queries using pymongo.

04: Analysis:
Use dataAnalysis.ipynb to analyze data from the mongoDB. 

05: Front End (Future):
Using HTML,CSS,JS to show data in an interactive format.

