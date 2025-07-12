# Task 1 – Cloud Storage Configuration on AWS S3

##  Task Objective:
To create and configure a secure cloud storage bucket on AWS S3, upload sample files, and manage access permissions.

---

##  Implementation Details:

###  S3 Bucket:
- Bucket Name: `secure-storage-nandini`
- Region: `ap-south-1` (Mumbai)
- Public Access: **Blocked (default settings)**
- Versioning: Disabled
- Default Encryption: **Enabled** (SSE-S3 – AES-256)

###  Uploaded Files:

The following files were uploaded to the S3 bucket as part of the cloud storage task:

- `CLOUD COMPUTING.pdf` – A PDF file used to test larger file upload
- `hello-codetech.txt` – A sample text file to verify storage and access
- `category_image.jpg` – An image file uploaded to test object visibility and format support


These files were uploaded to the bucket using the AWS Management Console.

###  Permissions:
- **Access Blocked Publicly**: All public access was blocked for secure storage
- **Access Control**: IAM-based permissions were configured instead of bucket policies
- **No public read access was granted**, keeping all files private

###  Encryption:
- Server-Side Encryption (SSE) was enabled
- Encryption Method: **SSE-S3 (AES-256)**
- Ensures that every file uploaded to the bucket is automatically encrypted at rest by AWS

---

##  Screenshots (included in `screenshots/` folder):
- `s3-bucket.png` – Bucket creation confirmation
- `upload-proof.png` – Uploaded files listed in the bucket
- `encryption-settings.png` – Default encryption settings (SSE-S3 enabled)

---

##  Outcome:
A secure and encrypted cloud storage bucket was successfully created on AWS S3 with appropriate access control and encryption measures in place.

---

##  Tools Used:
- AWS S3 Console
