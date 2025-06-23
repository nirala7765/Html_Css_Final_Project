# 🌐 Static Website CI/CD on AWS S3

This project demonstrates a fully automated **CI/CD pipeline** using **AWS CodePipeline**, **CodeBuild**, and **S3 static website hosting** to deploy a static HTML/CSS/JS website.  
Every time code is pushed to the GitHub repo, the website is automatically built and deployed.

---

## 🚀 Live Website

**👉 [View Live Site](http://website-deployment7765.s3-website-us-east-1.amazonaws.com/)**  
Hosted via S3 Static Website Hosting (us-east-1)

---

## 📁 Project Structure

├── buildspec.yml
├── index.html
├── stylesheet.css
├── clock.svg
├── Styling.c
├── img/

🔄 How the CI/CD Pipeline Works
Source: GitHub repository is connected as the source.

Build: CodeBuild reads buildspec.yml and prepares the site files.

Deploy: Output artifacts are pushed to the S3 bucket configured for static website hosting.

Live: Site is available instantly at the public S3 URL.

🛠 AWS Services Used
S3 – Static Website Hosting

CodePipeline – CI/CD automation

CodeBuild – Build & artifact packaging

IAM – Secure roles for pipeline and build

(Optional) Route 53 + CloudFront for domain and SSL

🔐 IAM Role Permissions
CodePipeline Role:

codepipeline.amazonaws.com trust

Permissions: S3 access, CodeBuild access

CodeBuild Role:

codebuild.amazonaws.com trust

Permissions: Read GitHub, write to S3

🧪 Testing the Deployment
To test the pipeline:

Make a small change to index.html

Commit and push to GitHub

Watch the pipeline trigger and deploy

Refresh the live site to see the update

📸 Screenshots 
Screenshots can be found in root directory 



![CodePipeline Setup](./screenshots/pipeline-setup.png)
![Live Website](./screenshots/live-site.png)
📜 License
This project is licensed under the MIT License.

🙋 Author
Arun Kumar
GitHub


