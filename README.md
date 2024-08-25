# Project-Career-page
A career page created form flask framework hosted on AWS EC2 and saves uploaded resumes to S3 and uses self created tls certs for accessing through https

# Steps -
- Create 2 EC2 instances
  - Application server (Install dependencies and host application code on this from ([this repo](https://github.com/RayanAhmed2000/aws-live-project))
    - steps :
        - lauch ubuntu ec2
        - create a SG allowing HTTP/HTTPS/SSH/MYSQL
        - ssh into server
        - Clone the application code on server -  git clone https://github.com/RayanAhmed2000/aws-live-project.git
        - install dependencies
          ```
          sudo apt-get install python3
          sudo apt-get install python3-flask
          sudo apt-get install python3-pymysql
          sudo apt-get install python3-boto3
          ```
        -  
  - Databse Server (Install mysql on this server and create a user grant him root privlidges)
