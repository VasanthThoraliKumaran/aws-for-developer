## Regions and az overview
![3 AWS Regions each of which has 3 Availability Zones](https://digitalcloud.training/wp-content/uploads/2022/02/aws-regions-availability-zones.png)

## AWS Regions
- a region is a which is a physical location around the world where a cluster data centers present.
- AWS has regions all around the world.
- Names starts with us-east-1, eu-west-3, etc.,
- Most of the aws services are region scoped.
- AWS maintains multiple regions such as North America, South America, Europe, China, Asia Pacific, South Africa, and the Middle East.

## How to choose a region
- **Compliance** with data governance and legal
    - eg: requirements:- data never leaves a region without your explicit permission
- **Proximity** to customers: reduced latency
- **Available services within a Region** new services and new features aren’t available in every Region
- **Pricing** pricing varies region to region and is transparent in the service pricing page.

## Availability Zones
- az are available into the region. We call each group of logical data centers an Availability Zone.
- az's are more discrete data centers with redundant power, networking, and connectivity in an AWS Region
- each region has many az's which are isolated, 
  - (usually 3, min is 3, max is 6). Example:
      - ap-southeast-2a
      - ap-southeast-2b
      - ap-southeast-2c
- Each availability zone (AZ) is one or more discrete data centers with redundant power, networking, and connectivity
- They’re separate from each other, so that they’re isolated from disasters
- They’re connected with high bandwidth, ultra-low latency networking

## AWS Point Of Presence (Edge Locations)
- AWS Point of Presence (PoP) is a physical location that serves as a connection point between AWS and local network providers, enabling faster data transfer.
- AWS Edge Locations, on the other hand, are distributed caching endpoints that store and serve content closer to end users, improving the performance of content delivery.
- Both play a crucial role in optimizing network performance and delivering AWS services efficiently to users around the world.
- Amazon has 400+ Points of Presence (400+ Edge Locations & 10+
Regional Caches) in 90+ cities across 40+ countries
- Content is delivered to end users with lower latency

### Diagram shows CloudFront (AWS's content delivery network (CDN)) Edge locations
![Edge Locations and Regional Edge Caches](https://digitalcloud.training/wp-content/uploads/2022/02/aws-cloudfront-edge-cache.png)

## Local Zones
- LZ's places compute, storage, database, and other select AWS services closer to end-users. 
- With AWS Local Zones, you can easily run highly-demanding applications that require single-digit millisecond latencies to your end-users.
- With LZ's, You can seamleslly run apps such as media & entertainment content creation, real-time gaming, reservoir simulations, electronic design automation, and machine learning.

## AWS Wavelength

- AWS Wavelength is a service provided by Amazon Web Services that brings the power of AWS closer to mobile devices by placing compute and storage infrastructure at the edge of the mobile network. In simpler terms, it enables developers to run their applications and services closer to where mobile users are located.
- This is particularly useful for real-time or latency-sensitive applications, such as gaming, video streaming, and augmented reality (AR). 
- AWS Wavelength brings AWS services to the edge of the 5G network, minimizing the latency to connect to an application from a mobile device.

## AWS Outpost
- AWS Outposts is a service provided by Amazon Web Services that allows you to have your own piece of Amazon's cloud infrastructure in your own data center. 
- It lets you run certain AWS services and use familiar tools on your own hardware, giving you a hybrid cloud experience. It's a way to bring some of the benefits of the AWS cloud to your own premises.

### Original reference [Aws Global Infrastructure](https://aws.amazon.com/about-aws/global-infrastructure/)