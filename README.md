# bikopt.com personal training website
This website will be used by Biko Ploeger to promote his personal lifestyle coaching business.

## Website deployment strategy
An AWS codepipeline is used to automatically deploy the website to a s3 bucket. 
The content of this bucket is then served to anyone visiting https://bikopt.com by AWS cloudfront. 
Any changes commited to the master branch will automatically be pushed to the s3 bucket at:
https://bikopt2.s3.eu-central-1.amazonaws.com/index.html
Changes may take up to 24 hours to be published to the cloudfront locations. 
