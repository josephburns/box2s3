box2s3

a brutish hack to move files from box.com to an AWS s3 bucket.  move all files matching a certain pattern from box.net to a desired s3 bucket/path.  uses oauth2 in an unnatural way since their api v2 requires it.      
tested with ruby 1.9.3

###usage###
ruby box2s3 pattern_to_match s3_bucket_name path_within_s3_bucket

###stuff that must be done before executing###
-install any of the gems you don't already have (net/http, mechanize, json, httparty, aws-sdk)
-configure your AWS credentials (left in single file for simplicity)
-create an app here: http://developers.box.net/ 
-get your client_id and client_secret for oauth2 within the app you created, add this to your configuration within the script 
-configure your box.com username/password within the script

###license###
(MIT)[http://opensource.org/licenses/MIT]
