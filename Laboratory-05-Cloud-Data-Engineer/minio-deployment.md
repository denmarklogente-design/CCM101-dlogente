# MinIO Deployment Documentation

## Deployment Summary

In this laboratory activity, I deployed MinIO as an object storage server using Docker in the KillerCoda Ubuntu Playground. After starting the MinIO container, I accessed its web console, created a bucket, and uploaded a sample file.

## Docker Command

The exact Docker command used to deploy the MinIO server was:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" quay.io/minio/minio server /data --console-address ":9001"
