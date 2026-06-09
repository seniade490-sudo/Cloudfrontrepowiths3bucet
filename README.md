# Cloudfrontrepowiths3bucet
AWS
<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Deliver a Website Globally with CloudFront

**Project Link:** [View Project](https://learn.nextwork.org/projects/6472bc81-e05d-4a5b-86b7-4692d40b3b86)

**Author:** Oluwaseni Oguntonade  
**Email:** seniade490@gmail.com

---

![Image](https://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/6472bc81-e05d-4a5b-86b7-4692d40b3b86_ig6jef1b)

## Project Overview: Building a Global CDN-Powered Website

### What this project builds and why it matters

In this project, I'm building a static portfolio website hosted on Amazon S3 and accelerated by Amazon cloudfront's global edge network, secured with HTTPS and Origin Access controls buckets... so that I would have a static website hosted privately in amazon S3 bucket, accessible only through cloudfront, A cloudfront distribution delivering my content from 750+ edge  locations worldwide with HTTPS enabled automatically, A cache invalidation that proves I understand how cdn update to Propagate to the edge. 

## Setting Up AWS Tools and CLI Access

### Goals for this setup step

In this step, I'm setting up an AWS account and installing the AWS CLI on windows, and configure it with my credentials so that I can interact with AWS services from terminal.

![Image](https://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/6472bc81-e05d-4a5b-86b7-4692d40b3b86_51n07o1h)

### CLI region and output configuration

I configured my CLI with region us-east-1 ... and output format would be in json...

## Creating a Private S3 Bucket as the Origin

### Goals for this setup step

In this step, I'm setting up a private S3 bucket in the us-east-1 region. so that I can write and upload a portfolio HTML page with CSS styling and also ensuring the bucket stays completely private.

![Image](https://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/6472bc81-e05d-4a5b-86b7-4692d40b3b86_nqvhjkdu)

### Why the S3 bucket stays private

The bucket is configured with private and not public access... which means any view on a webserver would be denied...

## Deploying a CloudFront Distribution with Origin Access Control

### Goals for this setup step

In this step, I'm setting up a cloudfront distribution that acts as the global front door to my bucket... so that I can use Origin Access Control (OAC) to securely read from your private bucket, so no one touches my S3 directly.

![Image](https://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/6472bc81-e05d-4a5b-86b7-4692d40b3b86_yleklemh)

### How OAC secures the origin

OAC allows CloudFront to access my S3 bucket with out making it public... without making my bucket public...

## Verifying CDN Caching in Action

### Goals for this testing step

In this step, I'm testing how CDN caching works in real time, inspecting response headers to identify the serving edge location... so that I can verify how to load my website through cloudfront https url and use browser developer tools... I would Access my portfolio through the CloudFront HTTPS endpoint, Observe cache hit and miss behavior across multiple requests

### Cache hits vs. cache misses explained

A cache hit means A cache hit means the file was served from a server geographically close to you.

## Updating Content and Invalidating the Edge Cache

### Goals for this invalidation step

In this step, I'm updating my portfolio page and re-upload it to S3. so that I can observe stale content served from CloudFronts's edge cache. I would create a cache invalidation to push updates to all edge locations.

![Image](https://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/6472bc81-e05d-4a5b-86b7-4692d40b3b86_9a1pl7nk)

### Why stale content persists after an S3 update

The old version appeared because CloudFront loads cached items from edge close to me, A cache invalidation tells CloudFront to discard cached copies so the next request fetches fresh content from S3 ...

## Advanced CDN: Custom Error Pages and Per-File Cache Behaviors

![Image](https://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/6472bc81-e05d-4a5b-86b7-4692d40b3b86_vqwqy5iz)

### Optimizing cache TTLs for CSS vs. HTML

In this project extension, I configured my CSS cache behavior with CloudFront, Cache behaviors let you apply different caching rules to different URL patterns, while it can serve your CSS files from cache for up to a week before checking your S3 bucket for updates. Since CSS changes are infrequent, this dramatically reduces origin load.... 

## Reflections and Key Takeaways

### Tools and concepts mastered

The key tools I used include S3 bucket, CloudFront, invalidation, error pages, distribution, ... Key concepts I learnt include cashing stays for over 24hrs, S3buckets replaces your html code as long as you upload a new one...

### Time and challenges

This project took me approximately the whole day... The most challenging part was always loading the cache, till i got to the tutors point of invalidation */...

### Looking ahead

I did this project today to learn how to use cloud cdn... Another skill I want to learn is Cloud Nat...

---

*Built with [NextWork](https://learn.nextwork.org) - [View this project](https://learn.nextwork.org/projects/6472bc81-e05d-4a5b-86b7-4692d40b3b86)*



<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Deliver a Website Globally with CloudFront

**Project Link:** [View Project](https://learn.nextwork.org/projects/6472bc81-e05d-4a5b-86b7-4692d40b3b86)

**Author:** Oluwaseni Oguntonade  
**Email:** seniade490@gmail.com

---

![Image](https://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/6472bc81-e05d-4a5b-86b7-4692d40b3b86_ig6jef1b)

## Project Overview: Building a Global CDN-Powered Website

### What this project builds and why it matters

In this project, I'm building a static portfolio website hosted on Amazon S3 and accelerated by Amazon cloudfront's global edge network, secured with HTTPS and Origin Access controls buckets... so that I would have a static website hosted privately in amazon S3 bucket, accessible only through cloudfront, A cloudfront distribution delivering my content from 750+ edge  locations worldwide with HTTPS enabled automatically, A cache invalidation that proves I understand how cdn update to Propagate to the edge. 

## Setting Up AWS Tools and CLI Access

### Goals for this setup step

In this step, I'm setting up an AWS account and installing the AWS CLI on windows, and configure it with my credentials so that I can interact with AWS services from terminal.

![Image](https://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/6472bc81-e05d-4a5b-86b7-4692d40b3b86_51n07o1h)

### CLI region and output configuration

I configured my CLI with region us-east-1 ... and output format would be in json...

## Creating a Private S3 Bucket as the Origin

### Goals for this setup step

In this step, I'm setting up a private S3 bucket in the us-east-1 region. so that I can write and upload a portfolio HTML page with CSS styling and also ensuring the bucket stays completely private.

![Image](https://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/6472bc81-e05d-4a5b-86b7-4692d40b3b86_nqvhjkdu)

### Why the S3 bucket stays private

The bucket is configured with private and not public access... which means any view on a webserver would be denied...

## Deploying a CloudFront Distribution with Origin Access Control

### Goals for this setup step

In this step, I'm setting up a cloudfront distribution that acts as the global front door to my bucket... so that I can use Origin Access Control (OAC) to securely read from your private bucket, so no one touches my S3 directly.

![Image](https://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/6472bc81-e05d-4a5b-86b7-4692d40b3b86_yleklemh)

### How OAC secures the origin

OAC allows CloudFront to access my S3 bucket with out making it public... without making my bucket public...

## Verifying CDN Caching in Action

### Goals for this testing step

In this step, I'm testing how CDN caching works in real time, inspecting response headers to identify the serving edge location... so that I can verify how to load my website through cloudfront https url and use browser developer tools... I would Access my portfolio through the CloudFront HTTPS endpoint, Observe cache hit and miss behavior across multiple requests

### Cache hits vs. cache misses explained

A cache hit means A cache hit means the file was served from a server geographically close to you.

## Updating Content and Invalidating the Edge Cache

### Goals for this invalidation step

In this step, I'm updating my portfolio page and re-upload it to S3. so that I can observe stale content served from CloudFronts's edge cache. I would create a cache invalidation to push updates to all edge locations.

![Image](https://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/6472bc81-e05d-4a5b-86b7-4692d40b3b86_9a1pl7nk)

### Why stale content persists after an S3 update

The old version appeared because CloudFront loads cached items from edge close to me, A cache invalidation tells CloudFront to discard cached copies so the next request fetches fresh content from S3 ...

## Advanced CDN: Custom Error Pages and Per-File Cache Behaviors

![Image](https://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/6472bc81-e05d-4a5b-86b7-4692d40b3b86_vqwqy5iz)

### Optimizing cache TTLs for CSS vs. HTML

In this project extension, I configured my CSS cache behavior with CloudFront, Cache behaviors let you apply different caching rules to different URL patterns, while it can serve your CSS files from cache for up to a week before checking your S3 bucket for updates. Since CSS changes are infrequent, this dramatically reduces origin load.... 

## Reflections and Key Takeaways

### Tools and concepts mastered

The key tools I used include S3 bucket, CloudFront, invalidation, error pages, distribution, ... Key concepts I learnt include cashing stays for over 24hrs, S3buckets replaces your html code as long as you upload a new one...

### Time and challenges

This project took me approximately the whole day... The most challenging part was always loading the cache, till i got to the tutors point of invalidation */...

### Looking ahead

I did this project today to learn how to use cloud cdn... Another skill I want to learn is Cloud Nat...

---

*Built with [NextWork](https://learn.nextwork.org) - [View this project](https://learn.nextwork.org/projects/6472bc81-e05d-4a5b-86b7-4692d40b3b86)*

