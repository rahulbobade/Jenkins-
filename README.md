# Change_jenkins_home 

#### By default, jenkins_home lives in ~/. jenkins. /var/lib/jenkins  When you start jenkins, it looks for an environment variable to tell it where to find those files . 

### By default 

![jenkins](https://user-images.githubusercontent.com/43333447/71321945-254bee80-24e7-11ea-9f68-4afd1e10d077.PNG)

### step 1) - Move jenkins directory 

---
       mv /var/lib/jenkins /Rahul/jenkins 

---

### Step 2) - Create symlink 

---
        ln -s /Rahul/jenkins /var/lib/jenkins

---
### Step 4) Set environment variable 

---
    export JENKINS_HOME=/Rahul/jenkins

    for check 

    export | grep -i jenkins 

    Then edit file vim /root/.bash_profile
    
![env](https://user-images.githubusercontent.com/43333447/71322084-40b7f900-24e9-11ea-9382-07647ca7ae99.PNG)

---
### Step 5) Update Env variable.

---
       source /root/.bash_profile

---       
### Step 6) Edit file vim /etc/sysconfig/jenkins

---
       Edit line no 10 

---

![upda](https://user-images.githubusercontent.com/43333447/71322186-d0aa7280-24ea-11ea-90d5-4cc234d55849.PNG)


### Step 7) Restart jenkins 

---
             systemctl stop jenkins 
             systemctl start jenkins 

---             

![jenkins after](https://user-images.githubusercontent.com/43333447/71322233-60e8b780-24eb-11ea-8c4a-eeef0820c53b.PNG)








