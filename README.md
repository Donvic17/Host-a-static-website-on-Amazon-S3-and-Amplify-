# Host-a-static-website-on-Amazon-S3-and-Amplify-
This is a Step-by-Step guide to hosting a static website using Amazon S3 and AWS Amplify

Tech Stack
- Amazon Amazon S3 (Simple Storage Service)
- AWS Amplify
- Amazon Route 53 (optional)

Steps

1. Prepare Your Static Website Files:
Ensure all your website files (HTML, CSS, JavaScript, images, etc.) are ready and organized in a local directory. Your main entry file should typically be named index.html.

2. Configure S3 for Static Website Hosting:
a. Create an S3 Bucket:
Open the AWS S3 console and create a new bucket. Choose a globally unique name.
Important: Disable "Block all public access" settings during bucket creation or modify them afterward to allow public access for static website hosting.
b. Enable Static Website Hosting:
In your S3 bucket's properties, navigate to "Static website hosting" and enable it.
Specify index.html as the "Index document." You can also specify an "Error document" if desired.
c. Upload Website Files:
Upload all your static website files to this S3 bucket.
d. Set Bucket Policy:
Go to "Permissions" in your S3 bucket and edit the "Bucket policy." Add a policy that grants public read access to your objects.

3. Deploy with AWS Amplify (Optional, but Recommended for Advanced Features):
a. Create a New App in Amplify:
Open the AWS Amplify console and choose "Host a web app."
