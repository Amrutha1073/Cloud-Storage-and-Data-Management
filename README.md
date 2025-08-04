# ☁️ Cloud Storage and Data Management Project

This project demonstrates the use of **Amazon S3** (or Google Cloud Storage) for organizing, securing, and retrieving data in the cloud. It is a part of the internship/project assignment under the topic **Cloud Storage and Data Management**.

---

## 📌 Objective

To create and manage a cloud storage bucket with features like folder structuring, access control, versioning, and data retrieval.

---

## 🛠️ Tools & Services Used

- **Amazon Web Services (AWS S3)**
- AWS Console or AWS CLI
- Screenshots and documentation
- Optional: GitHub for version control

---

## ✅ Tasks Performed

1. Created an S3 Bucket for cloud storage.
2. Organized files into logical folders (e.g., `/images`, `/documents`).
3. Configured public/private access permissions using bucket policies.
4. Enabled **versioning** to track and restore old versions.
5. Uploaded files and demonstrated retrieval using object URLs.
6. Took screenshots of each step for documentation.

---

## 🖼️ Screenshots

| Action | Screenshot |
|-------|------------|
| Bucket Creation | ![Bucket Creation](screenshots/bucket_creation.png) |
| Folder Structure | ![Folder Structure](screenshots/folder_structure.png) |
| Access Permissions | ![Access](screenshots/access.png) |
| Versioning Enabled | ![Versioning](screenshots/versioning.png) |
| File Retrieval | ![File Retrieval](screenshots/retrieval.png) |

---

## 🔒 Access Control Example

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::your-bucket-name/*"
    }
  ]
}
