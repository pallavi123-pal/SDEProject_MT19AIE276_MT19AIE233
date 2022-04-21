# SDEProject_MT19AIE276_MT19AIE233
SDE Project

AUTHOR - PALLAVI(MT19AIE276) & DEVIDATT JOSHI(MT19AIE233)

To run SQLFlow on a desktop computer running Windows, Linux, or macOS, follow below steps:
 step-1: install VirtualBox (v6.1.6 is recommended)
 
  step-2: download the released VirtualBox .ova file from following link:
  http://cdn.sqlflow.tech/latest/SQLFlowPlaygroundFull.ova
  
  Step3: Configure virtual machine & Import .ova File:
  RAM:8gb, Processores: 4 cores, Video Memory: 16mb, Graphics Controller: VMSVGA
  
  Step4: Start VM & wait until Ubantu bionic login appear.
  
  Step5: enter username:root and passwor:sqlflow.
  
  step6:Once logged in execute ./start.bash command, the script to start SQLFlow playground.
  
  step7: once minikube,kubernetl, argo server are depolyed and started then open jyupiter notebook.
  
  Step8: after completing step 7: open notebook using folloing address: http://localhost:8888
  
  Step9:  select Classify Iris Dataset Using DNNClassifer notebook and execute.
  
  Step10: Install MySQL db and import heart.csv into MySQL table using below 2 queries:
          
          CREATE TABLE heart 
          (
            age INT,
            sex INT,
            cp INT,
            trestbps INT,
            chol INT,
            fbs INT,
            restecg INT,
            thalach INT,
            exang INT,
            oldpeak DECIMAL(2 , 1),
            slope INT,
            ca INT,
            thal INT,
            target INT
          );  

          LOAD DATA INFILE 'C:/ProgramData/MySQL/MySQL Server 8.0/Uploads/heart.csv' INTO TABLE heart FIELDS TERMINATED BY ',' IGNORE 1 ROWS;
  
  Step11: import the Bagging_Boosting.ipnyp in jupyter notebook. Connect to db and Run the cells in sequence
