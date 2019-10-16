# How to use AWS, AMAZON WEB SERVICE

- note to self (always ensure you do not upload your ssh file)


## setting up AWS

- login to AWS
- create ec2 instance with all the settings required

##  unzipping dos2unix and sending files to VM

- mv the dos2unix.exe to /bin/
- go into the place with provision.sh file on gitbash
- enter command

      dos2unix.exe provision.sh

- move that provision file to

      scp -i path/to/key file/to/copy user@ec2-xx-xx-xxx-xxx.compute-1.amazonaws.com:path/to/file

    - fill in the blanks to the

- moved the app directory using the same code
  - remember to -r <dir>


## SSH ubuntu

    ssh -i path/to/AccessKey.pem ubuntu@ec2-12-34-567-890.compute-1.amazonaws.com

- ec2-12-34-567-890.compute-1.amazonaws.com = DNS is found in the instance in aws website.

- find the provision.sh file
  - ./provision.sh
- find the app folder
  - npm Install
  - npm start
