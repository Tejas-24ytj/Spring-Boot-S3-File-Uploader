# S3 File Storage using Spring Boot

## Description
This is a Spring Boot application for uploading, deleting, and downloading files to/from an AWS S3 bucket. The application provides REST endpoints to interact with the S3 bucket.

![Screenshot 2024-05-03 120536](https://github.com/Tejas-24ytj/Spring-Boot-S3-File-Uploader/assets/105742352/f6d253dc-7110-4a76-9677-fc336b018ffa)

![Screenshot 2024-05-03 120402](https://github.com/Tejas-24ytj/Spring-Boot-S3-File-Uploader/assets/105742352/ec613171-8581-461b-9930-c240806f9fd7)

![Screenshot 2024-05-03 115846](https://github.com/Tejas-24ytj/Spring-Boot-S3-File-Uploader/assets/105742352/63b0e0be-5103-4371-9abe-cfdeacbc84f1)



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
