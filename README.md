# Offline installation for SLO Simply Smarter

## 1) Download ZIP
on linux or windows and un zip file

https://github.com/JLLormeau/slo_simply_smarter_offline/archive/refs/heads/main.zip


## 2) Create an `APi-Token` with this scope :

 - Access problem and event feed, metrics, and topology
 - Read configuration 
 - Write configuration
 - Read SLO
 - Write SLO
 
  
## 3) Automatic installation and update with `python script`
Prerequisite : requests installed 
 
    python 3.6+
    pip install requests
 
Apply these variables
     
    export MyTenant=domaine.com/e/abcd12234 for managed (without https://...)
    export MyToken=dt0c01.1234ABCD.XXXX
    export Owner=smarter (optional - no need to define this user in the UI)

Run the script

    python3 Deploy_and_Update_SLO_Simply_Smarter.py
    
   ![image](https://user-images.githubusercontent.com/40337213/211930107-21d89c32-55fa-4dfb-a36d-6ce6b1182ffb.png)  
  
 The `SLO simply smarter` is installed 

 
