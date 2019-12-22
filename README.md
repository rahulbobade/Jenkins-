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
        ls -s /Rahul/jenkins /var/lib/jenkins

---
### Step 4) Set environment variable 

---
    export JENKINS_HOME=/Rahul/jenkins

    for check 

    export | grep -i jenkins 

    Then edit file vim /root/.bash_profile
![env](https://user-images.githubusercontent.com/43333447/71322084-40b7f900-24e9-11ea-9382-07647ca7ae99.PNG=1000*1000)



---
