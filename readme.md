To Create an EC@ instance first install the Java Development Kit and then proceed to install Jenkins

Install Java: 'sudo apt install default-jdk'.

Install Jenkins: 'sudo apt install jenkins'

![Screenshot (44)](https://github.com/shiyammk/Jenkins-ci-cd/assets/160907011/b8422d82-f5e8-452f-a75f-50e4b34c690e)

![Screenshot (46)](https://github.com/shiyammk/Jenkins-ci-cd/assets/160907011/04fc0fbd-6749-4d5a-b61b-5575037dcfa9)

Connect to the port 8080 and Install Docker

Install Docker: 'sudo apt install docker.io -y'

![Screenshot (45)](https://github.com/shiyammk/Jenkins-ci-cd/assets/160907011/d8a05aef-5a17-41ad-bdf0-d8512107309d)

![Screenshot (49)](https://github.com/shiyammk/Jenkins-ci-cd/assets/160907011/4fd859d8-c55a-4878-9395-1e5ebf2d266a)

Copy the Instance's public IP,paste it into the browserand then log in to Jenkins

![Screenshot (48)](https://github.com/shiyammk/Jenkins-ci-cd/assets/160907011/39fd11f2-ec68-40ae-b273-9f9afb885721)

Create an IAM role and attach it to the EC2 Instance

![Screenshot (52)](https://github.com/shiyammk/Jenkins-ci-cd/assets/160907011/f8c40547-9032-4b88-b911-8658bf66d186)

![Screenshot (53)](https://github.com/shiyammk/Jenkins-ci-cd/assets/160907011/3e5bacc5-ae33-40a8-a33a-36cd872d8524)

Create a Jenkins Pipeline and configure it then Create the Amazon Elastic Container Registry(ECR) and paste its URL into Jenkins

--> git clone clone repository

   cp -r ./repository name/* .
   
   sudo docker build . -t your tag name
   
   paste it retrives a token from ECR
   
   sudo docker tag test paste your ECR URL
   
   sudo docker push paste your ECR URL
   
   sudo docker run -d -p 80:80 paste your ECR URL 

   Ten build on Jenkins Project
   
![Screenshot (51)](https://github.com/shiyammk/Jenkins-ci-cd/assets/160907011/3edb02da-8279-4092-93ef-dbfaae8dc351)

![Screenshot (58)](https://github.com/shiyammk/Jenkins-ci-cd/assets/160907011/e3e3b34d-d779-437c-89b1-6a138d753f53)

![Screenshot (59)](https://github.com/shiyammk/Jenkins-ci-cd/assets/160907011/a8f4742a-ca7e-4a9a-bc12-334bc07968ba)

Finally copy your public IP and paste it on Browser

Final output in jenkins

![Screenshot (60)](https://github.com/shiyammk/Jenkins-ci-cd/assets/160907011/11ce3be9-01ce-4be9-b5e1-919e3bc1b58d)



