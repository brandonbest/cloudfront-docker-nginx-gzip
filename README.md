# gzip on Cloudfront Using nginx
Event after enabling "compression" in Cloudfront, HTML is passed from Cloudfront to the end user in plain, uncompressed text.

We need to tweek some nginx settings to push compressed HTML into Cloudfront. Luckily, it's a simple conf update.
