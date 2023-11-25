<h1>Password Manager Hosted In AWS</h1>

![Password-Manager](https://github.com/MMease/Password-Manager/assets/42321472/7629f2db-a37f-4189-9239-826ee0f61f61)

<h2>Prerequisites for Password Manager in Cloud</h2>

- Creating an AWS Account (https://aws.amazon.com)
- Download Oracle VM VirtualBox (https://www.virtualbox.org/wiki/Downloads)
- Download Unbuntu (https://ubuntu.com/download/desktop)
  - Ensure you download Ubuntu 22.04.2 LTS
- Buy a domain name (https://www.namecheap.com)
  - This step is optional for longterm use 


<h2>Getting Started with Password Manager</h2>

1. Go to https://www.passbolt.com & click on "On-perm install"

<img width="1792" alt="Passbolt 1" src="https://github.com/MMease/Password-Manager/assets/42321472/249d330e-3d13-4d7b-8c98-cee3808582a9">


2. Next, select "Free Download" under the Community section  

<img width="1792" alt="Passbolt 2" src="https://github.com/MMease/Password-Manager/assets/42321472/59bbc466-3efc-4e27-b3ef-0b43593e0cf9">


3. Select "AWS" for deploying on cloud provider.

<img width="1792" alt="Passbolt 3" src="https://github.com/MMease/Password-Manager/assets/42321472/340eb218-b048-4c75-a95f-15ec08374f40">

<h3>AWS Passbolt Setup</h3>

1. After hitting deploy to AWS, You will see this page. Click the "Subscribe" button.

![AWS Adding passbolt](https://github.com/MMease/Password-Manager/assets/42321472/056d1dc8-3b8f-4533-951f-f9851f702280)

2. Configure the Passbolt. Once finished click "Countinue to Lunch".

![AWS Passbolt Configuration   Launch](https://github.com/MMease/Password-Manager/assets/42321472/14574ce4-1459-40e3-898e-8fe9a01777c1)

3. Creating a Securtiy Group in AWS

![AWS Passbolt Launch (Security Group Creation)](https://github.com/MMease/Password-Manager/assets/42321472/6b4dade1-5f0c-4bc4-9c80-ad7632d4bec8)

4. Creating a Key Pair 

![Imported key ](https://github.com/MMease/Password-Manager/assets/42321472/4b925729-3155-4a59-85bb-f7430e54b735)

- Generate the Key pair using Ubuntu's terminal
  - Copy the key and post it in AWS
    
![Linux key generator](https://github.com/MMease/Password-Manager/assets/42321472/ba59f83d-1478-43e5-be0a-e89ee9866196)

- This is how it looks when a pair is successfully added. After its added, lunch to the EC2.

![Added Keypair](https://github.com/MMease/Password-Manager/assets/42321472/99666bb5-cb70-4520-959c-a342b6aa3f2e)


<h4>Lunching EC2 Insatnce</h4>

- This is an EC2 instance created in the EC2 Console.
  
![EC2 Instance](https://github.com/MMease/Password-Manager/assets/42321472/b3d5db96-02ed-4d91-b8a5-072318f5a5ba)

- A IP address is assigned to the instance.
- Paste the Public IPv4 to the Search bar and then you can access the Password Manager.

![EC2 Instance Summary](https://github.com/MMease/Password-Manager/assets/42321472/71d4577c-400f-4877-8532-4b07bcd9ebef)

<h5>Configure & Host PassBolt</h5>

- Run the initial system check (It will Fail)
- Configure the database for the Manager.
  - Create Admin account

![Passbolt database Configure ](https://github.com/MMease/Password-Manager/assets/42321472/8fcce13f-a3a3-4c10-80e9-2846872a5671)

- This is your Password Managers homepage. Your all done!!!!

![Final Password Mager in AWS](https://github.com/MMease/Password-Manager/assets/42321472/b592303e-1690-4bf9-b8c5-9961518ac8e9)
