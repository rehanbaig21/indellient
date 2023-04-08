# S3 Uploader



## Install Dependencies

install inotify-tools in your desired OS (I have used Ubuntu)
  - sudo apt update
  - sudo apt install inotify-tools

## Steps to setup CLI Program

-  Download, extract or clone the github repository, move this code to your local Directory
-  cp S3uploader to your desired location from cloned github repo
   - eg ( cp ./S4uploader /Users/<username>/Documents/S3uploader)
-  edit file permission executable as following
   - chmod +x /Users/<username>/Documents/S3uploader
-  add followig line under your .bash_profile to add path to s3 uploader in to your PATH variable
   - export PATH=$PATH:/Users/<username>/Documents/S3uploader
-  export aws profile to point to right aws account where files suppose to be uploaded
   - export AWS_PROFILE= <aws-profile-name>
   
## Usage

Pass  argument as following

- s3uploader (S3BUCKETNAME) (OBSOULUTE PATH OF FILE TO MONITOR)
  - s3uloader mybcuketname //Users/<username>/Documents/myfile.txt
