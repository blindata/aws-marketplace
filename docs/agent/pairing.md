---
layout: default
title: Pairing Agent with Blindata Core
parent: Agent
nav_order: 2
last_modified_date: 2021-02-26T16:12
---

# Pairing with Blindata Core

---

<div style="display: flex; flex-direction: row-reverse; align-items: flex-start;">
    <div style="flex-grow: 1;">
        <p style="font-weight: bold">On this page:</p>
        <ul>
            <li>
                <a href="#find-credentials-by-checking-the-system-log-on-aws-management-console" style="white-space: break-spaces;">
                    Find credentials by checking the system log on AWS Management Console
                </a>
            </li>
            <li>
                <a href="#find-credentials-by-connecting-to-your-application-instance-using-ssh" style="white-space: break-spaces;">
                    Find credentials by connecting to your application instance using SSH
                </a>
            </li>
        </ul>
    </div>
    <div style="flex-grow: 2; margin-right: 1.5em;">
        <p>Application credentials allow you to log in to your new Blindata Data Governance and Compliance Platform.</p>
        <p>These credentials consist of a username and password. The username is set by default.  The password is randomly generated during the first boot of the instance.</p>
        <p>There are two options for obtaining your application password:</p>
        <ol>
            <li>Checking the system log on AWS Management Console</li>
            <li>Connecting to your application instance through SSH</li>
        </ol>
    </div>
</div>


## Find credentials by checking the system log on AWS Management Console

- Log in to the AWS Management Console.
- Navigate to the EC2 dashboard.
- In the left navigation bar, click the “Instances > Instances” menu item.
- Select your instance. Please be sure to switch to the region where your instance was launched.
- Use the instance actions menu to navigate to the “Monitor & troubleshoot > Get system log” menu item.
- Review the system log until you find the application password. You will also find the default username.

<div style="padding: 8px; border-radius: 3px; margin: 0.75rem 0px 0px; display: flex; align-items: baseline; background-color: rgb(255, 250, 230);">
    <span><img src="{{site.baseurl}}/assets/images/warning.png" style="width: 24px; max-width: none; padding-right: 8px"></span>
    <span>We strongly recommend that you chance the application password as soon as possible for security reason. You can change the application credentials (username and password) within the application settings.</span>
</div>


## Find credentials by connecting to your application instance using SSH

The application credentials are stored in a standalone file. To obtain the credentials at any time, follow these instructions:
- Connect to the application instance through SSH.
- Run the following command to see your application credentials:

```sh
sudo cat /home/blindata/blindata_credentials.conf
```

<div style="padding: 8px; border-radius: 3px; margin: 0.75rem 0px 0px; display: flex; align-items: baseline; background-color: rgb(255, 250, 230);">
    <span><img src="{{site.baseurl}}/assets/images/warning.png" style="width: 24px; max-width: none; padding-right: 8px"></span>
    <span>We strongly recommend that you chance the application password as soon as possible for security reason. You can change the application credentials (username and password) within the application settings.</span>
</div>

---
