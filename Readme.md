1. Deploy App
`sls deploy`

Note: You might need to update the bucket name in `serverless.yml`


2. Download an mp4 and upload it to the desired bucket.
```shell
curl -OL https://archive.org/download/mov-bbb/mov_bbb.mp4

aws s3 cp mov_bbb.mp4 s3://YOURBUCKETNAME/mov_bbb.mp4

# wait a little bit….
aws s3 cp s3://YOURBUCKETNAME/mov_bbb.mp4.gif mov_bb.mp4.gif
```

## References:

- https://www.serverless.com/blog/publish-aws-lambda-layers-serverless-framework


