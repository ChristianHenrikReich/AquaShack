# AquaShack
This is a pico-example of a meta-data driven lakehouse for Microsoft Fabric.

## Installation 

/Setup.ipynb holds all to get started. It is one script, to setup the full example.

NB! 2025-02-07: There has been fixed a concurrency issue, where transformations could leak data to other transformations. 
                There is tiny minor risc of experince this. Re-running the /Setup.ipynb notebook fixes this. 

## Documentation

AquaShack is traditionel medallion architecture, due to history the Bronze, Silver and Gold layers are named Landing, Base and Curated.

When installed, the notebook 1_AquaShack_Landing_To_Base will move example data from Landing to Base. 
The notebook 2_AquaShack_Base_To_Curated will move data from Base to Curated.

![image](https://github.com/user-attachments/assets/470adae5-d49d-4ffd-a23e-49cf29e1f1ec)

