# Offline installation for SLO Simply Smarter

## 1) Create an `APi-Token` with this scope :

 - Access problem and event feed, metrics, and topology
 - Read configuration 
 - Write configuration
 - Read SLO
 - Write SLO
 - User sessions(*)
 - Read metrics(*)
 - Write metrics(*)
 - Ingest Metrics(*) 
   
  ![image](https://user-images.githubusercontent.com/40337213/210615861-e34ab003-df23-455f-9513-2d1ac63a4759.png)  
  (*) optionnel for BizOps only ([detail](https://dynatrace.github.io/BizOpsConfigurator/index.html#prerequisites))  

  
## 2) Automatic installation and update with `script python`
Prerequisite : requests installed 
 
    python 3.6+
    pip install requests
 
Apply these variables
     
    export MyTenant=domaine.com/e/abcd12234 for managed (without https://...)
    export MyToken=dt0c01.1234ABCD.XXXX
    export Owner=smarter (optional - no need to define this user in the UI)
       
    python3 Deploy_and_Update_SLO_Simply_Smarter.py
    
   ![image](https://user-images.githubusercontent.com/40337213/211930107-21d89c32-55fa-4dfb-a36d-6ce6b1182ffb.png)  
  
 The `SLO simply smarter` is installed 

 
