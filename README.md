## EXPERIMENT 5
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
2.	Locate Default encryption. 
3.	Record the encryption type. 
Possible configurations include:
•	SSE-S3 
•	SSE-KMS 
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
<img width="959" height="437" alt="1" src="https://github.com/user-attachments/assets/48d45480-6e2d-4c2d-87e5-444770d04597" />

<img width="959" height="433" alt="2" src="https://github.com/user-attachments/assets/5786f3dc-c66d-49e5-901c-dc0e4a045868" />

<img width="959" height="432" alt="3" src="https://github.com/user-attachments/assets/121fa715-8ef3-454a-81c5-30077d3f4c2f" />

<img width="959" height="433" alt="4" src="https://github.com/user-attachments/assets/ade173e2-e07a-45db-9066-402bb9fcc732" />

<img width="959" height="438" alt="5" src="https://github.com/user-attachments/assets/fa8145b0-5675-4482-95cf-099710e7ca37" />

<img width="959" height="437" alt="6" src="https://github.com/user-attachments/assets/bdc4facb-41f7-4085-9b26-97db597700fe" />

<img width="959" height="431" alt="7" src="https://github.com/user-attachments/assets/4b095708-11a1-4f10-8368-fb668691fab3" />

<img width="959" height="435" alt="8" src="https://github.com/user-attachments/assets/1ce40911-9e08-4a69-af49-0c857b0a46be" />

<img width="959" height="434" alt="9" src="https://github.com/user-attachments/assets/7279acb7-6ef5-498e-9836-a4cc6a3b7613" 
/>

<img width="959" height="440" alt="10" src="https://github.com/user-attachments/assets/2d7b7e3f-b5cc-476b-a4ce-eb0631295a84" />

<img width="959" height="437" alt="11" src="https://github.com/user-attachments/assets/8455bd7e-08e1-4c0a-b286-6fb15bc6e7c7" />

## Result:
All AWS user activities, including volume creation, deletion, and permission changes, were successfully audited using CloudTrail.
