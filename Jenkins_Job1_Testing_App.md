# Creating a CICD(e) Pipeline Localhost -> Git -> Jenkins -> AWS

## Task 
- Create a localhost
- Assign it to a git repo
- Create a secure channel between localhost and git repo
- Create webhook
- Create Jenkins job to test application


## Step 1: Generate SSH key pair

- Generate an ssh key pair in .ssh folder with: (for windows) `ssh-keygen -t -C "<your_email>"`
- This will generate a public (id_rsa.pub) and private (id_rsa) key 

## Step 2: Secure SSH Connection by Adding Public Key to Your GitHub Repo

- Copy the content of the id_rsa.pub 

![image](https://user-images.githubusercontent.com/14828358/145586456-566c3c63-b8dd-496a-a55d-be720b06d056.png)


- On the git repo you want to connect with: `Setting` -> `Deploy keys` -> `Add deploy`

![image](https://user-images.githubusercontent.com/14828358/145585263-470520cc-d714-4420-9351-505078528c8a.png)

