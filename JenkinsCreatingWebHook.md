
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

![image](https://user-images.githubusercontent.com/14828358/145388926-79b91786-2d0f-4e15-80b1-9d2ed7d36381.png)


- click allow write access box
- click add key



![image](https://user-images.githubusercontent.com/14828358/145387498-8c7df23d-2cbd-407e-9eaf-67c0dcc424c2.png)

![image](https://user-images.githubusercontent.com/14828358/145390483-fa2251b6-e1a6-4fcd-b08d-50fa8ad2e0db.png)

![image](https://user-images.githubusercontent.com/14828358/145390524-d0223c95-155f-4253-a38d-f09f24f1d202.png)


## Test Commands on agent node

![image](https://user-images.githubusercontent.com/14828358/145390765-66463f13-ab70-43db-8771-b9f961425779.png)

get ssh

![image](https://user-images.githubusercontent.com/14828358/145390912-119c8afe-00be-4262-b3cf-18b9364ced63.png)

![image](https://user-images.githubusercontent.com/14828358/145391501-2c84d485-c7d7-4abc-b07e-224b32b6334b.png)

![image](https://user-images.githubusercontent.com/14828358/145391325-f19c4e6f-6c0d-4633-b661-e7e43225cfd2.png)

![image](https://user-images.githubusercontent.com/14828358/145391447-1665c4d2-f914-4406-bd4f-f36509bd93fc.png)







