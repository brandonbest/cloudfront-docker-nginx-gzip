# gzip on Cloudfront Using nginx
Event after enabling "compression" in Cloudfront, HTML is passed from Cloudfront to the end user in plain, uncompressed text.

## Why this works
Nginx does not apply compression on proxied requests by default. Cloudfront passes Nginx the header `Via` in the request - which tells Nginx it's a proxied request. The configuration update allows compression on all request types.
