Traffic Mirroring on AWS VPC

Traffic Mirroring is an Amazon VPC feature that you can use to copy network traffic from an elastic network interface of Amazon EC2 instances. You can then send the traffic to out-of-band security and monitoring appliances for:
• Contentinspection 
• Threatmonitoring 
• Troubleshooting

The security and monitoring appliances can be deployed as individual instances, or as a fleet of instances behind a Network Load Balancer with a UDP listener. Traffic Mirroring supports filters and packet truncation, so that you only extract the traffic of interest to monitor by using monitoring tools of your choice.

The following are the key concepts for Traffic Mirroring:
• Target—The destination for mirrored traffic.
• Filter—A set of rules that defines the traffic that is copied in a traffic mirror session.
• Session—An entity that describes Traffic Mirroring from a source to a target using filters.




