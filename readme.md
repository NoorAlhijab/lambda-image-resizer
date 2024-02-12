# Serverless Lambda Function for Image Resizing

This project showcases a Lambda function that automatically resizes images when they are uploaded to an S3 bucket. The Lambda function is triggered by S3 events and processes the images to create resized thumbnails, which are then stored in a separate S3 bucket.

## Project Flowchart

![Project Flowchart](/images/flowchart-image.png)

## How it Works

1. **Bucket Configuration:** Two S3 buckets are used: one for original images and one for resized thumbnails.

2. **Lambda Setup:** Create the Lambda function and configure execution roles with necessary S3 access permissions.

3. **Lambda Code:** Write code to fetch original images, resize them using the Sharp library, and store thumbnails in the destination bucket.

4. **Testing:** Test the Lambda function using simulated S3 put events to verify automatic resizing.

5. **Trigger Configuration:** Add a trigger to the Lambda function using S3 bucket events to trigger resizing upon image upload.

### Install Dependencies

To install the required dependencies for this project, run the following command in your terminal:

```bash
npm install sharp


## Technologies Used

- AWS Lambda
- AWS S3
- Sharp (Image Processing Library)
- Node.js
