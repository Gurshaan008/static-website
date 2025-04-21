# OVERVIEW
This project demonstrates how to host a static website to AWS S3 and serve it globally with the help of cloudfront. It also integrates CI/CD automation with the help of Github Actions to auto deploy changes when the code is pushed to the repository.

# TECHNOLOGIES USED
- HTML/CSS (Static site)
- AWS S3 (Website Hosting)
- AWS cloudfront (CDN)
- Github Actions (CI/CD Automation)

# PROJECT STRUCTURE

-static-website/
-|
-|--- index.html
-|--- style.css
-|___ .github/
-   |___ workflows/
-       |___ deploy.yml

GitHub Repo (Push) 
   ↓
GitHub Actions 
   ↓
AWS CLI Sync → S3 Bucket 
   ↓
CloudFront (Cache Invalidation)
   ↓
User Gets Updated Website Globally
