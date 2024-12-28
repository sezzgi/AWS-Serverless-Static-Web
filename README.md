# Aws-serverless-static-web

Serverless web application deployment showcasing AWS cloud architecture with CloudFront, S3, and Route 53, implemented using Infrastructure as Code.

## Project Highlights

✨ Serverless Architecture  
✨ Content Delivery Network Integration  
✨ Custom Domain Configuration  
✨ SSL/TLS Security  
✨ Infrastructure as Code


## Key Features

• Cloud-Native Architecture
  - Serverless hosting with S3
  - Global content delivery
  - Automated SSL/TLS
  - DNS management
  - Zero maintenance

• Security Implementation
  - HTTPS enforcement
  - Custom SSL certificates
  - S3 bucket policies
  - Secure content delivery


## Quick Start

1. **Prerequisites**
   ```bash
   - AWS Account
   - AWS CLI configured
   - Domain in Route 53
   ```

2. **Deploy**
   ```bash
   # Deploy infrastructure
   aws cloudformation create-stack \
     --stack-name static-web \
     --template-body file://template.yml \
     --parameters \
       ParameterKey=DomainName,ParameterValue=yourdomain.com \
       ParameterKey=FullDomainName,ParameterValue=app.yourdomain.com

   # Upload content
   ./upload-script.sh
   ```

3. **Access**
   - Website will be available at your configured domain
   - CloudFront provides global content delivery
   - Automatic HTTPS enforcement
  
