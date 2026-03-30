# 🔐 AWS S3 Security: SSE-S3 Encryption & Pre-Signed URLs

## 📌 Project Overview

This project demonstrates how to secure an Amazon S3 bucket by enabling default encryption (SSE-S3) and sharing private objects securely using time-limited pre-signed URLs.

---

## 👤 Author

**Name:** Poonam Langote
**Assignment:** Task 7 – Enable Default SSE-S3 Encryption & Generate Pre-Signed URLs
**Submission Date:** 30/03/2026
**AWS Region:** us-east-1

---

## 🎯 Objective

* Enable **default encryption (SSE-S3)** on an S3 bucket
* Keep the bucket **private**
* Generate **secure, temporary access** using pre-signed URLs

---

## 🚀 Steps Performed

### 1️⃣ Create Private S3 Bucket

* Bucket Name: `secure-bucket-poonam`
* Region: `us-east-1`
* Keep **Block all public access** enabled

---

### 2️⃣ Enable Default Encryption

* Go to **Properties → Default Encryption**
* Select **SSE-S3 (Amazon S3 managed keys)**
* Save changes

---

### 3️⃣ Upload File

* Upload a file (e.g., `index.html`)
* Verify encryption:

  * Go to **Object → Properties**
  * Confirm **Server-side encryption: SSE-S3**

---

### 4️⃣ Verify Private Access

* Copy Object URL
* Open in browser → ❌ **Access Denied**
* Confirms bucket is private

---

### 5️⃣ Generate Pre-Signed URL

* Select object → **Object Actions → Share with pre-signed URL**
* Set expiry: **5 minutes**
* Copy URL

---

### 6️⃣ Test Pre-Signed URL

* Open URL → ✅ File accessible
* Wait 5 minutes → ❌ Access Denied (URL expired)

---

## 🔐 Key Concepts

### 🔸 SSE-S3 Encryption

* Automatically encrypts data at rest
* Managed by AWS (no key management needed)

### 🔸 Pre-Signed URL

* Temporary access to private objects
* Controlled by time expiration
* Useful for secure file sharing

---

## ✅ Results

* Private S3 bucket successfully created
* Default encryption (SSE-S3) enabled
* Direct object access blocked
* Pre-signed URL provided temporary access
* URL expired as expected after set time

---

## 📷 Screenshots

* Bucket creation
* Encryption settings
* Access denied (private bucket)
* Pre-signed URL working
* Expired URL access denied

---

## 📚 Conclusion

This project demonstrates how to secure S3 data using encryption and controlled access. Pre-signed URLs provide a powerful way to share private content securely without exposing the bucket publicly.

---
