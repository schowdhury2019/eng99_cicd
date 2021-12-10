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

- Paste the content into the Key text box
- Click `Allow write access`
- Click `Add key`

![image](https://user-images.githubusercontent.com/14828358/145586821-bdd9ad4a-94fe-4fa8-8990-8c1f5aa621fe.png)

# Step 3: Add Webhook

- Webhooks allow intereaction between web-based applications through the use of custom callback. 
- In this case, we weant to allow git to automaticaly communicate with Jenkins whenever work has been pushed onto the git repo (dev branch)
- `Settings` -> `Webhooks` -> `Add webhook`

![image](https://user-images.githubusercontent.com/14828358/145588542-fa4aff4b-781a-45a3-88e3-b580177bbc6b.png)

- Add the custom webhook url into the Payload URL box

![image](https://user-images.githubusercontent.com/14828358/145589068-2001a47e-fe64-4026-bc1b-ed3c5261fea9.png)


# Step 4: Jenkins Jobs

- Create a new job on jenkins
- `New Item` -> `Freestyle Project`

![image](https://user-images.githubusercontent.com/14828358/145590556-320d7a4d-881e-4c0e-b525-9da794d55d1d.png)

![image](https://user-images.githubusercontent.com/14828358/145590718-8efa9eca-5013-42ad-be90-a9cb467f86a4.png)

























