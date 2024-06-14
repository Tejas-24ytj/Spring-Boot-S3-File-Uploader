# S3 File Storage using Spring Boot

## Description
This is a Spring Boot application for uploading, deleting, and downloading files to/from an AWS S3 bucket. The application provides REST endpoints to interact with the S3 bucket.

![Screenshot 2024-05-03 120616](https://github.com/Tejas-24ytj/Spring-Boot-S3-File-Uploader/assets/105742352/aa961fa4-7c78-42d6-be51-0a8103f29001)


## Prerequisites
Before running the application, you need to:
- Manually create an S3 bucket on AWS.
- Create an IAM role with S3 full access permissions.
- Generate an Access Key ID and Secret Access Key for the IAM role.

## Dependencies
Make sure to add the following dependencies to your `pom.xml`:

```xml
<!-- AWS Java SDK -->
<dependency>
    <groupId>com.amazonaws</groupId>
    <artifactId>aws-java-sdk</artifactId>
    <version>1.11.486</version>
</dependency>

<!-- Spring Cloud Starter AWS -->
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-starter-aws</artifactId>
</dependency>


# AWS Credentials
cloud.aws.credentials.access-key=<Your-Access-Key-ID>
cloud.aws.credentials.secret-key=<Your-Secret-Access-Key>

# AWS Region
cloud.aws.region.static=<Your-AWS-Region>

# S3 Bucket Name
cloud.aws.s3.bucket=<Your-S3-Bucket-Name>

You can customize this template according to your specific application structure, requirements, and preferences. Make sure to replace placeholders like `<Your-Access-Key-ID>`, `<Your-Secret-Access-Key>`, `<Your-AWS-Region>`, and `<Your-S3-Bucket-Name>` with your actual AWS credentials and S3 bucket information.
