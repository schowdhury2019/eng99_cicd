
# Creating a Webhook with SSH Key

- eng99_jenkins.pub on github
- eng99_jenkins private key

Once access is allowed, jenkins will clone everything on a master server
Tests will be run on an agent node

send a request from jenkins to aws cloud, need aws secure key to ssh into ec2 instance

add ssh rule from jenkins IP in instance security group

![image](https://user-images.githubusercontent.com/14828358/145381694-d7874cc0-898e-4bdc-8f17-d510d7a19702.png)

public key on git repo

![image](https://user-images.githubusercontent.com/14828358/145386524-d8790539-af45-4ba9-b4df-e6cc54d4246d.png)

- Generate public and private key


![image](https://user-images.githubusercontent.com/14828358/145387297-70162a45-7849-40b0-9764-d4d197b28d9e.png)


![image](https://user-images.githubusercontent.com/14828358/145387218-905e9326-2195-4099-8696-ced4722653ea.png)

- Paste public key into text box, 
- click give write permission box
- click add key

![image](https://user-images.githubusercontent.com/14828358/145387498-8c7df23d-2cbd-407e-9eaf-67c0dcc424c2.png)
