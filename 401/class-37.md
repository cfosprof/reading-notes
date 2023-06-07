Introduction to Amazon S3

What is Amazon S3?
A scalable, secure, and durable object storage service that offers cost effective ways to store and retrieve any amount of data.

List at least 3 features that it offers to its users.
Scalability, security, durability

What is an object key?
A unique identifier for an object in S3. It's a string of up to 1024 characters.


[S3 with Amplify](https://docs.amplify.aws/lib/storage/getting-started/q/platform/android/)

1. Which dependencies are needed to install Amplify AWS S3 to your android application?
2. implementation 'com.amplifyframework:aws-storage-s3:2.8.4'
3. 
4. What is needed in order to upload data to your bucket?
5. A new amplify storage object, and a call to the upload method, with an object key and the data to be uploaded.
6. 
7. what method(s) initialize(s) the Amplify Auth and Storage categories?
8. Amplify.configure