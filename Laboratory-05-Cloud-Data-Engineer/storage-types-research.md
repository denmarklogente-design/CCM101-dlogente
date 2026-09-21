# Storage Types Research

## Comparison of Cloud Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in separate blocks that can be attached to a virtual machine and used similar to a hard drive. | Operating systems, databases, and applications that require fast disk access. | AWS EBS |
| File Storage | Stores files in folders and directories and allows them to be accessed over a network. | Shared documents, media files, and applications that need shared file access. | AWS EFS |
| Object Storage | Stores data as individual objects with metadata and unique identifiers inside containers called buckets. | Images, videos, backups, documents, and other unstructured data. | Amazon S3 |

## Why Object Storage Is Suitable for Millions of User-Uploaded Images

Object Storage is suitable for millions of user-uploaded images because it is designed to store large amounts of unstructured data. Each image can be stored as an individual object inside a bucket, making it easier for applications to organize and retrieve many files.
