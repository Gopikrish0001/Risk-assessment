# Risk-assessment## 
# EX.NO : 5
# REG.NO:212223043001

## ASSET-ORIENTED RISK ASSESSMENT OF STORAGE ASSETS IN AWS AND AZURE
## Objective:
   To identify storage assets in AWS S3 and Microsoft Azure Blob Storage, identify possible vulnerabilities and threats, and assess their likelihood, impact, and risk level.

## 1. Software / Cloud Services Required
•	AWS Account 
•	Microsoft Azure Account 
•	Web Browser 
•	Internet Connection
## Cloud Services Used
## Cloud Platform	Storage Service
AWS	Amazon S3
Microsoft Azure	Azure Blob Storage
PART A — AWS S3 STORAGE ASSESSMENT
## Step 1: Login to AWS
1.	Open the AWS Management Console. 
2.	Sign in using your AWS account. 
3.	Search for S3. 
4.	Select Amazon S3. 

## Step 2: Select the S3 Bucket
1.	Click Buckets. 
2.	Select the S3 bucket created in the previous experiment. 
3.	Record: 
o	Bucket name 
o	AWS Region 
o	Number/type of objects 
Screenshot: S3 bucket overview.

## Step 3: Check Block Public Access
1.	Open the S3 bucket. 
2.	Select Permissions. 
3.	Locate Block public access (bucket settings). 
4.	Check Block all public access. 
Record:
•	ON → Secure configuration 
•	OFF → Potential public-access risk 
Screenshot: Block Public Access settings.

## Step 4: Check Bucket Versioning
1.	Select the Properties tab. 
2.	Locate Bucket Versioning. 
3.	Record whether it is: 
o	Enabled 
o	Disabled 
Security purpose
Versioning helps recover previous versions of objects after accidental deletion or modification.
Screenshot: Bucket Versioning.

## Step 5: Check Default Encryption
1.	Stay in the Properties tab. 
•	DSSE-KMS 
Security purpose
Encryption protects stored data from unauthorized disclosure.
Screenshot: Default Encryption.

## Step 6: Check Bucket Policy
1.	Select Permissions. 
2.	Locate Bucket policy. 
3.	Check whether a bucket policy exists. 
Record:
•	Policy exists 
•	No policy 
Note
A missing bucket policy is not automatically a vulnerability. Access may be controlled through IAM and other AWS security mechanisms.
Screenshot: Bucket Policy section.

## Step 7: Check Object Ownership and ACL
1.	In Permissions, locate Object Ownership. 
2.	Record the current configuration. 
A common secure configuration is:
Bucket owner enforced
This means:
•	ACLs are disabled. 
•	Objects are owned by the bucket owner. 
•	Access is controlled using policies. 
Screenshot: Object Ownership.

## Step 8: Check Server Access Logging
1.	Go to Properties. 
2.	Locate Server access logging. 
3.	Record whether it is: 
o	Enabled 
o	Disabled 
Security purpose
Logging helps investigate suspicious or unauthorized access to the bucket.
Screenshot: Server Access Logging

## OUTPUT:

<img width="1851" height="1015" alt="Screenshot 2026-09-01 143007" src="https://github.com/user-attachments/assets/fb430c9e-905e-4f1d-bfbf-20ff1b2ae0a3" />

<img width="1856" height="1021" alt="Screenshot 2026-09-01 143033" src="https://github.com/user-attachments/assets/21337be5-c5df-4f79-8afb-7814ff49b687" />

<img width="1846" height="1017" alt="Screenshot 2026-09-01 143414" src="https://github.com/user-attachments/assets/d2cd9401-a1a6-4857-8147-356a97394411" />

<img width="1855" height="1016" alt="Screenshot 2026-09-01 143207" src="https://github.com/user-attachments/assets/b372d49a-085d-42a2-bcc6-05695a5ad614" />

<img width="1847" height="1020" alt="Screenshot 2026-09-01 143349" src="https://github.com/user-attachments/assets/9d5708d6-4b06-4c77-a7a5-56a3c4a44fa5" />

<img width="1602" height="1017" alt="image" src="https://github.com/user-attachments/assets/425d44ee-7ba5-4c64-aa33-d797031056eb" />

## Result:
All AWS user activities, including volume creation, deletion, and permission changes, were successfully audited using CloudTrail.


