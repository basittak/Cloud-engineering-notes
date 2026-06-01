# Deploying a Static Website to S3 + CloudFront

1. Create an S3 bucket with public access for static hosting or use CloudFront to restrict public S3 access.
2. Upload index.html to the bucket: `aws s3 cp index.html s3://my-bucket/`
3. (Optional) Create a CloudFront distribution and point the origin to the S3 bucket.
4. Invalidate CloudFront cache when updating: `aws cloudfront create-invalidation --distribution-id <id> --paths "/index.html"`

Troubleshooting
- Check bucket policy and object ACLs
- Review CloudFront logs and S3 access logs
