# UT Course Scraping


This is a python script created to parse through a set of class names at UT Austin, search them up in the course registration webpage, and output that information onto an excel spreadsheet. This will be primarily useful for those hoping to constantly check the status of classes, as it removes the need to search up each class individually manually.

##### courses.txt
This is the file the script reads the list of classes to search up

Example formatting:
```
M 427J
M 427L
E M 306
C S 313E
```

##### course listing.py
There are four parameters that need to be changed here

PATH: This will be the path to your chrome web driver, which can be installed here https://chromedriver.chromium.org/downloads
COURSE_WEBSITE: This is the link to the semester course schedule   
USERNAME: Your UT EID  
PASSWORD: Your password  

After these are filled out, ensure that all the required libraries are installed, and it should be ready to run. Everything will be automated besides the Duo Mobile Verification. The output will be saved into an excel file named output.xlsx

Columns
1: Unique Number
2: Professor
3: Course Status
4: Days
5: Hours

At the bottom, there is a list of all the professors teaching the courses.

Changing the sheets will show the results for the different classes
