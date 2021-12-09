
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




![image](https://user-images.githubusercontent.com/14828358/145391738-f6fb6f88-8059-4376-9294-88d35aadd136.png)

![image](https://user-images.githubusercontent.com/14828358/145391784-4896d3b4-8912-43bd-bca7-f6b46129611b.png)


![image](https://user-images.githubusercontent.com/14828358/145391873-40eeca68-2828-45f1-9e72-b2d426e8d5bb.png)

![image](https://user-images.githubusercontent.com/14828358/145391926-b335954e-8479-4e38-92a2-41d1e2d530a4.png)

![image](https://user-images.githubusercontent.com/14828358/145392130-631022f9-a47c-421a-a752-8019cd2911b3.png)

Apply and Save

Build Now

![image](https://user-images.githubusercontent.com/14828358/145392330-20677fd0-e1a1-4279-9b70-8c2f657f7abc.png)


jenkins clones everything from github using the ssh pipeline we allowed

![image](https://user-images.githubusercontent.com/14828358/145394100-aa6044fb-e5c9-45d0-bf11-00abfacf3eb5.png)



Configure webhook to always listen to github so it pulls any changes

![image](https://user-images.githubusercontent.com/14828358/145395210-1e7cd0a3-a0ec-4a93-8661-ea6999d049df.png)


![image](https://user-images.githubusercontent.com/14828358/145395612-3281fbe4-9e45-477a-be4a-45364132c030.png)


![image](https://user-images.githubusercontent.com/14828358/145395783-742ad273-ae3c-4e8a-82c4-30c3356d6f92.png)
