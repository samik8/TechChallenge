# TechChallenge
Source Code Files:

Applications:
1. TechChallenge_AuthSource.xml
2. SS_System.xml
3. RK_System.xml

CorrelationConfig:
Identity_Correlation.xml

Rules:
1. Auth Source Customization Rule.xml
2. Inactive Rule.xml
3. RK Deprovisioning.xml
4. RK Provisioning.xml
5. SS After Provisioning Rule.xml
6. SS Deprovisioning.xml
7. SS Provisioning.xml
8. Status Rule.xml

Bundle:
1. RK_MODIFY
2. RK_READ
3. RK_REMOVE

IdentityTrigger
Leaver.xml

TaskDefinition
1. AccountAggregation-Authoritative.xml
2. AccountAggregation-RK.xml
3. AccountAggregation-SS.xml

Workflow:
1. LeaverWorkflow.xml
2. Schedule-Leaver Subprocess.xml


Deployment of the code:

1. Pull the code from the git repository.
2. Import source code xml and replace following macros from the target.properties
     %%auth_file_path%%=/home/spadmin/Desktop/Files/TechChallenge_AuthSource.csv
     %%query_rk%%=select * from rk_system;
     %%pwd_rk%%=1:xDikd6BMwY+LL9iXETAjBg==
     %%query_ss%%=select * from ss_system;
     %%pwd_ss%%=1:xDikd6BMwY+LL9iXETAjBg==
