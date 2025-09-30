# 🔘Deploying The Auto-scalling🔘


## ⚪introduction
### Target Group
A *Target Group* is a logical grouping of resources (like EC2 instances or containers) that receive incoming traffic from a load balancer.  
- You register servers (targets) such as EC2 instances or IP addresses.  
- The load balancer routes requests to these targets based on health checks and routing rules.  
- Targets can be added or removed without affecting the load balancer configuration.

### Auto Scaling Group (ASG)
An *Auto Scaling Group* automatically adjusts the number of compute resources to handle changes in traffic.  
- It launches or terminates EC2 instances based on defined scaling policies.  
- Ensures the desired number of instances is always running (high availability).  
- Helps optimize costs by scaling down during low demand and scaling up when traffic increases.

### Load Balancer
A *Load Balancer* distributes incoming network traffic across multiple targets to improve availability and reliability of your application.  
- It prevents any single server from becoming a point of failure.  
- Types in AWS include *Application Load Balancer (ALB), **Network Load Balancer (NLB), and **Gateway Load Balancer (GWLB)*.  
- Works seamlessly with Target Groups and Auto Scaling Groups for dynamic, fault-tolerant architectures.


step 1. Launch this 3 template


<img width="1909" height="859" alt="Screenshot (49)" src="https://github.com/user-attachments/assets/93f71b03-d3e2-4a37-ab39-d205a80c70a4" />



step 2. create 3 auto scalling group 


<img width="1911" height="859" alt="Screenshot (50)" src="https://github.com/user-attachments/assets/c5f46bd0-7948-474b-9a4f-6cfd292a6e0c" />


step 3. auto scalling group edit this schelude action 


<img width="1916" height="895" alt="Screenshot (51)" src="https://github.com/user-attachments/assets/648a2273-0fa0-42e4-8217-ad057e410684" />


step 4. create 3 target group 



<img width="1906" height="900" alt="Screenshot (52)" src="https://github.com/user-attachments/assets/0af08390-39ee-4e87-83c3-16b5a58d6e95" />



step 5. create a load balancer




<img width="1916" height="864" alt="Screenshot (53)" src="https://github.com/user-attachments/assets/9ac7d727-1ade-4050-946c-a86480da1a1b" />



step 6. auto scalling group attach to target group.1 mobile-ASG edit



<img width="1907" height="873" alt="Screenshot (57)" src="https://github.com/user-attachments/assets/7dafc9d7-6448-422f-a064-20ad17f94f10" />



attach to mobile-ASG target group



<img width="1920" height="911" alt="Screenshot (54)" src="https://github.com/user-attachments/assets/cc312efc-919e-4059-9968-1a7d872d5e8d" />




step 7. auto scalling group attach to target group.2 Laptop-ASG edit



<img width="1906" height="864" alt="Screenshot (58)" src="https://github.com/user-attachments/assets/a12e741a-6a88-402f-8c44-cd737c78c0bf" />



attach to mobile-ASG target group.



<img width="1907" height="864" alt="Screenshot (55)" src="https://github.com/user-attachments/assets/ea621933-5636-426c-a00e-8c8de9470366" />



step 8.auto scalling group attach to target group.3 Home-ASG edit



<img width="1903" height="864" alt="Screenshot (59)" src="https://github.com/user-attachments/assets/e4ac4bf4-d65e-41eb-8263-95e9ff623b85" />


attach to Home-ASG target group.


<img width="1920" height="913" alt="Screenshot (56)" src="https://github.com/user-attachments/assets/d4e4a149-6481-479e-92e4-5fe7871facc0" />



step 9. copy the DNS name


<img width="1911" height="749" alt="Screenshot (62)" src="https://github.com/user-attachments/assets/be8546ee-ceab-408f-a54d-a0b106ec8ae4" />



step 10. paste DNS name in browser 

<img width="1601" height="918" alt="Screenshot (60)" src="https://github.com/user-attachments/assets/ee540095-a188-47eb-8e29-9bc7e888ea4a" />


##📝 Summary
- **Target Group** → Defines where the traffic should go (set of targets).  
- **Load Balancer** → Distributes traffic across targets in a target group.  
- **Auto Scaling Group** → Manages scaling of EC2 instances to match demand.  

Together, they provide a **scalable, reliable, and fault-tolerant architecture** for modern cloud applications.  

---

