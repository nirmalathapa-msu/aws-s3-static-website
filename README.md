# aws-s3-static-website
Amazon Simple Storage Service (Amazon S3) can be used to host static Websites without a need for a Web server (at an extremely low cost). S3 buckets can be used to host the HTML, CSS and JavaScript files for entire static websites.



**Create an S3 Bucket**
When you first create an S3 bucket, you select the AWS Region in which the files will be geographically stored.
•	Click on "Create Bucket" button.
•	Provide a globally unique name for bucket and select Region.

![image](https://github.com/user-attachments/assets/fcae35e3-4539-46e3-b570-02045a188cf7)

**Upload Content of your Website**
Upload the website contents to your S3 bucket including sub-folders.
For Example: You can use sample Website "Website" folder contents (provided in this repository).

![image](https://github.com/user-attachments/assets/cc1efc75-cfd9-44c3-ae5c-4df32276db80)


**Add a Bucket Policy to allow Public Read Access**
Go to Permissions Tab and update Public Access Setting:
Uncheck Manage public bucket policies:
•	Uncheck - Block new public bucket policies (Recommended)
•	Uncheck - Block public and cross-account access if bucket has public policies (Recommended)

![image](https://github.com/user-attachments/assets/37186005-ab06-49a4-a42e-27e0a8bb74b2)


** Enable Website Hosting**
In order to serve assets via url, you need to enable Website Hosting
Go to Properties and enable "Static Website Hosting" option
Note the endpoint. http://{bucket-name}.s3-website-{AWS-Region}.amazonaws.com
![image](https://github.com/user-attachments/assets/72a4298a-b644-4bb6-b21f-d15ad083d3ab)



**Access Your Website (Testing/Validation)**
Access the site in browser: http://{bucket-name}.s3-website-{AWS-Region}.amazonaws.com
For Example: http://hosting-portfolio.s3-website.ap-south-1.amazonaws.com/



![image](https://github.com/user-attachments/assets/41dc9466-3fbd-4b06-a764-106b1e05a277)



