
# Creating a Webhook with SSH Key

- eng99_jenkins.pub on github
- eng99_jenkins private key

Once access is allowed, jenkins will clone everything on a master server
Tests will be run on an agent node

send a request from jenkins to aws cloud, need aws secure key to ssh into ec2 instance

add ssh rule from jenkins IP in instance security group

![image](https://user-images.githubusercontent.com/14828358/145381694-d7874cc0-898e-4bdc-8f17-d510d7a19702.png)
