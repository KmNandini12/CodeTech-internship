# Task 1 – Cloud Storage Configuration on AWS S3

##  Task Objective:
To create and configure a secure and functional cloud storage system using Amazon S3. The task involved uploading files, managing permissions, and enabling public access to demonstrate file availability.

---

##  Implementation Details:

###  S3 Bucket:
- **Bucket Name**: `secure-storage-nandini`
- **Region**: `ap-south-1` (Mumbai)
- **Public Access**: Partially enabled via bucket policy to allow public read access to objects
- **Versioning**: Disabled
- **Encryption**: Server-Side Encryption enabled (SSE-S3 – AES-256)

###  Uploaded Files:
The following files were uploaded to the S3 bucket:
- `CLOUD COMPUTING.pdf` – Internship guideline document
- `hello-codetech.txt` – Sample test file
- `category_image.jpg` – Image file for visibility demo

---

##  Permissions & Access Control:

- Initially, **block public access** was enabled.
- A custom **bucket policy** was added later to allow **public read access to all objects** in the bucket.
- IAM permissions were also tested separately in Task 4 (restricted access via user policy).

###  Public Object URLs:

- [hello-codetech.txt](https://codetech-internship-bucket.s3.ap-south-1.amazonaws.com/hello-codetech.txt)
- [category_image.jpg](https://codetech-internship-bucket.s3.ap-south-1.amazonaws.com/category_image.jpg)
- [CLOUD COMPUTING.pdf](https://codetech-internship-bucket.s3.ap-south-1.amazonaws.com/CLOUD+COMPUTING.pdf)

> These URLs are publicly accessible without needing authentication.

---

##  Encryption:
- **Type**: Server-Side Encryption with Amazon S3 managed keys (SSE-S3)
- **Status**: Enabled by default for all uploaded objects
- Ensures that data is automatically encrypted at rest

---

##  Screenshots (Uploaded Separately):
- `s3-bucket-overview.png` – Bucket list and access status
- `s3-file-uploads.png` – Uploaded object list
- `s3-policy-setting.png` – policy settings
- `file-details.png` – Object overview with access and encryption info

---

##  Outcome:
A fully functional S3 bucket was created and configured with public read access and encryption. Files were uploaded and verified to be securely stored and publicly accessible as per the internship requirements.

---

## 🛠 Tools Used:
- AWS Management Console (S3)
- Web browser (to verify public URLs)
