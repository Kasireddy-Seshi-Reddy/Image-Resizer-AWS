# Image-Resizer-AWS
I completed this AWS project of - Image Resizer Using S3 Buckets and Lambda Function, during my 7 Weeks Summer Training program (Cloud Computing using AWS) - Offered by GokboruTech (A Startup company in Punjab)


# Image Resizer Lambda

This Lambda will be invoked when a file is uploaded to a particular bucket. It will fetch the file that was added, resize it, and store the output in a different bucket.

## Run Locally

Clone the project

```bash
  git clone https://github.com/Kasireddy-Seshi-Reddy/Image-Resizer-AWS
```

Install Dependencies

```bash
# Required options if on mac
npm install --arch=x64 --platform=linux --target=16x sharp
```

## Environment Variables

Remember set the `DEST_BUCKET` in your Lambda's "Configuration" tab. To do this, open your Lambda in the AWS Console, select the "Configuration" tab, then click "Environment variables"

```bash
DEST_BUCKET=thumbnails-bucket-name
```

## Deployment

```bash
npm run package
```

Running the command above will zip your source code and dependencies. The zip can then be uploaded to your Lambda.
