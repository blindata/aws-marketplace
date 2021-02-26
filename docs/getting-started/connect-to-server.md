---
layout: default
title: Connect to the server using SSH
parent: Getting Started
nav_order: 3
last_modified_date: 2021-02-26T16:12
---

# Connect to the server using SSH

---

To log in your EC2 instance and execute commands on the server using the command line, you need an SSH client and the server credentials.

These credentials consist of an SSH username and a private key.

The SSH username you should use to access your instance is `ec2-user`.

The private key is the one of the key pair that you associated to your instance the first time you deployed the server

<div style="padding: 8px; border-radius: 3px; margin: 0.75rem 0px 0px; display: flex; align-items: baseline; background-color: rgb(222, 235, 255);">
    <span><img src="{{site.baseurl}}/assets/images/information.png" style="width: 24px; max-width: none; padding-right: 8px"></span>
    <span>Check the <a href="https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html">Amazon EC2 User Guide for Linux Instances</a> to know how the SSH keys can be created or uploaded on the AWS Management Console.</span>
</div>

<div style="padding: 8px; border-radius: 3px; margin: 0.75rem 0px 0px; display: flex; align-items: baseline; background-color: rgb(255, 250, 230);">
    <span><img src="{{site.baseurl}}/assets/images/warning.png" style="width: 24px; max-width: none; padding-right: 8px"></span>
    <span>If you did not associate a key pair with your EC2 instance or you lose the private key, you will not be able to log in to it. In this case, check the <a href="https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/replacing-lost-key-pair.html">Amazon EC2 User Guide for Linux Instances</a> or contact AWS support and follow their instructions to gain SSH access to your server.</span>
</div>