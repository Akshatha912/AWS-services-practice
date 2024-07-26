# AWS-services-practice
Working with VPC- NACL and Security groups

1)	Create a VPC  - select VPC and more
                           2 subnets and 2 availability zones

2)	Create EC2 instance – on Ubuntu machine
Edit network settings – attach the VPC that was created above
-	Select a public subnet and enable Auto –assign public IP
-	Launch instance
3)	Connect ec2 instance on Mobaxterm
4)	Update all packages – sudo apt update
5)	Install python application – python3 –m http.server 8000
6)	Edit inbound security rules under ec2 instance – to allow port 8000
![image](https://github.com/user-attachments/assets/e74e6b21-e27b-4102-a028-97260577170d)

7)	Edit inbound rules in NACL- lower rule number gets higher priority
![image](https://github.com/user-attachments/assets/bb8a52cb-edc6-4e6a-81bc-1043308c51c1)

8)	http://public_ip_of_ec2:8000 – redirected to the page in the below screenshot. This is a simple python3 application.
   ![image](https://github.com/user-attachments/assets/df90a0dc-c252-45ef-9306-1885b061f6f4)


