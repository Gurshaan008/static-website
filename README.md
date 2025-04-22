# OVERVIEW
In this project I'm hosting a static website to AWS S3 and serve it globally with the help of Cloudfront. I've also integrated CI/CD automation using Github Actions to auto deploy changes when the code is pushed to the repository.

# TECHNOLOGIES USED
- HTML/CSS (Static site)
- AWS S3 (Website Hosting)
- AWS cloudfront (CDN)
- Github Actions (CI/CD Automation)

# PROJECT STRUCTURE
```
static-website/
├── index.html
├── style.css
├── assets/
│   ├── CloudFront Settings/
│   │   ├── Clear-Cache.png
│   │   ├── Default-Root.png
│   │   └── Origin-S3.png
│   ├── GitHub Actions/
│   │   ├── Deploy.png
│   │   └── Deployment-Successful.png
│   ├── S3 settings/
│   │   ├── Allow-Public-Access.png
│   │   └── Static-Website-Hosting.png
│   └── Live-Website.png
└── .github/
    └── workflows/
        └── deploy.yml
```
        
# SCREENSHOTS INCLUDED
All images and screenshots related to this project are in the `assets/` folder. They are organized into subfolders based on functionality.
1) S3 Bucket Settings
2) CloudFront Settings
3) Github Action workflow
4) Successful GitHub Actions Run
5) Live Webiste (Final Output)

# HOW IT WORKS
1) You push the code to the 'main' branch
2) GitHub Actions triggers a workflow defined in '/github/workflows/deploy.yml'
3) It uses AWS CLI to syn the local project file to the S3 bucket
4) After uploading, it invalidates CloudFront cache to ensure new changes are visible immidiately

# CONCLUSION
- Hosting static website on AWS S3
- Configuring CloudFront with custom origins
- Automating deployments using GitHub Actions
- Cache invalidation for content delivery networks
