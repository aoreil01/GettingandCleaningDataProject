## variables

subject: unique number for each subject 1:30

label: a label name for each activity

                           "WALKING"
                           "WALKING_UPSTAIRS"
                           "WALKING_DOWNSTAIRS"
                           "SITTING"
                           "STANDING"
                           "LAYING"

the rest of the columns are from the embedded accelerometer and gyroscope from a smartphone (Samsung Galaxy S II)

"tbodyaccmeanx"            "tbodyaccmeany"           
"tbodyaccmeanz"            "tbodyaccstdx"             "tbodyaccstdy"             "tbodyaccstdz"            
"tgravityaccmeanx"         "tgravityaccmeany"         "tgravityaccmeanz"         "tgravityaccstdx"         
"tgravityaccstdy"          "tgravityaccstdz"          "tbodyaccjerkmeanx"        "tbodyaccjerkmeany"       
"tbodyaccjerkmeanz"        "tbodyaccjerkstdx"         "tbodyaccjerkstdy"         "tbodyaccjerkstdz"        
"tbodygyromeanx"           "tbodygyromeany"           "tbodygyromeanz"           "tbodygyrostdx"           
"tbodygyrostdy"            "tbodygyrostdz"            "tbodygyrojerkmeanx"       "tbodygyrojerkmeany"      
"tbodygyrojerkmeanz"       "tbodygyrojerkstdx"        "tbodygyrojerkstdy"        "tbodygyrojerkstdz"       
"tbodyaccmagmean"          "tbodyaccmagstd"           "tgravityaccmagmean"       "tgravityaccmagstd"       
"tbodyaccjerkmagmean"      "tbodyaccjerkmagstd"       "tbodygyromagmean"         "tbodygyromagstd"         
"tbodygyrojerkmagmean"     "tbodygyrojerkmagstd"      "fbodyaccmeanx"            "fbodyaccmeany"           
"fbodyaccmeanz"            "fbodyaccstdx"             "fbodyaccstdy"             "fbodyaccstdz"            
"fbodyaccjerkmeanx"        "fbodyaccjerkmeany"        "fbodyaccjerkmeanz"        "fbodyaccjerkstdx"        
"fbodyaccjerkstdy"         "fbodyaccjerkstdz"         "fbodygyromeanx"           "fbodygyromeany"          
"fbodygyromeanz"           "fbodygyrostdx"            "fbodygyrostdy"            "fbodygyrostdz"           
"fbodyaccmagmean"          "fbodyaccmagstd"           "fbodybodyaccjerkmagmean"  "fbodybodyaccjerkmagstd"  
"fbodybodygyromagmean"     "fbodybodygyromagstd"      "fbodybodygyrojerkmagmean" "fbodybodygyrojerkmagstd" 

n=68 columns

from each of these variables the mean and standard deviation was calculated.

## Transformation: aggr.data

All the values are means, aggregated over 30 subjects and 6 activities, 
The resulting dataset is 180 rows by 68 columns.
