Creating a bucket in S3 is one way to host files in a contained environment. They will all need a bucket name.

Make sure not to block public access, especially for DevOps classwork.

Enabling versioning lets you compare different versions of a file, but consumes more storage capacity.

Using the AWS address lets you access the files through a web browser, meaning containers can also be used to publish static web pages.


AWS can also generate access control for buckets with IAM. Set up an identity with IAM and restrict bucket access accordingly for more security.


Numerous objects you create using AWS can be managed by security groups. These groups control who can access what. Editing the inbound rules lets you manage what can access a bucket, EC2 instance or other items.