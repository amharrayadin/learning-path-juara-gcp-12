## ARC120

## Overview

In a challenge lab you’re given a scenario and a set of tasks. Instead of following step-by-step instructions, you will use the skills learned from the labs in the course to figure out how to complete the tasks on your own! An automated scoring system (shown on this page) will provide feedback on whether you have completed your tasks correctly.

When you take a challenge lab, you will not be taught new Google Cloud concepts. You are expected to extend your learned skills, like changing default values and reading and researching error messages to fix your own mistakes.

To score 100% you must successfully complete all tasks within the time period!

## Setup

### Before you click the Start Lab button

Read these instructions. Labs are timed and you cannot pause them. The timer, which starts when you click **Start Lab**, shows how long Google Cloud resources are made available to you.

This hands-on lab lets you do the lab activities in a real cloud environment, not in a simulation or demo environment. It does so by giving you new, temporary credentials you use to sign in and access Google Cloud for the duration of the lab.

To complete this lab, you need:

- Access to a standard internet browser (Chrome browser recommended).

**Note:** Use an Incognito (recommended) or private browser window to run this lab. This prevents conflicts between your personal account and the student account, which may cause extra charges incurred to your personal account.

- Time to complete the lab—remember, once you start, you cannot pause a lab.

**Note:** Use only the student account for this lab. If you use a different Google Cloud account, you may incur charges to that account.

## Challenge scenario

You recently started a new role as a Cloud Architect. One of your responsibilities is to build and operate web applications using Google Cloud.

### Your challenge

Your manager asked you to build a website to provide products and orders information. You are not asked to write code or scripts as it is another team's responsibility. Your job is to build infrastructure for the web application using Google Cloud. Here are the requirements:

- Create a new Cloud Storage bucket to store files.
- Create and attach a persistent disk to a Compute Engine virtual machine (VM) instance.
- Use Compute Engine to host a web application using a NGINX web server.

Some standards you should follow:

- Create all resources in the region and zone, unless otherwise directed.

Each task is described in detail below, good luck!

## Task 1. Create a Cloud Storage bucket

Your team has requested a new Cloud Storage bucket, so they can store their built code and startup scripts.

- Create a bucket named **\-bucket** (US multi-region).

Click _Check my progress_ to verify the objective. Create a Cloud Storage bucket

## Task 2. Create and attach a persistent disk to a Compute Engine instance

1.  Create a new Compute Engine instance named **my-instance** with the following configuration:

| Property        | Value                          |
| --------------- | ------------------------------ |
| Series          | E2                             |
| Machine type    | e2-medium                      |
| Boot disk type  | New balanced persistent disk   |
| Boot disk size  | 10 GB                          |
| Boot disk image | Debian GNU/Linux 12 (bookworm) |
| Firewall rules  | Enable **Allow HTTP traffic**  |

2.  Create a new persistent disk named **mydisk** with a size of 200GB.
3.  Attach the persistent disk to the instance.

Click _Check my progress_ to verify the objective. Create and attach a persistent disk to an instance

## Task 3. Install a NGINX web server

For this task, SSH into the Compute Engine instance, and install a NGINX web server. Here's a reminder of the general steps:

1.  Update the OS.
2.  Install NGINX.
3.  Confirm that NGINX is running.

Click _Check my progress_ to verify the objective. Install a NGINX web server

### Test the web application

To test the web application, return to the Cloud Console, and click the **External IP** link in the row for your machine name. Or, add the **External IP** value to `http://EXTERNAL_IP/` in a new browser window or tab.

A default web page should open with the message "Welcome to nginx!".

## Congratulations!

### Earn your next skill badge

This self-paced lab is part of the [The Basics of Google Cloud Compute](https://www.skills.google/course_templates/754) skill badge. Completing this skill badge earns you the badge above, to recognize your achievement. Share your badge on your resume and social platforms, and announce your accomplishment using #GoogleCloudBadge.

### Google Cloud training and certification

...helps you make the most of Google Cloud technologies. [Our classes](https://cloud.google.com/training) include technical skills and best practices to help you get up to speed quickly and continue your learning journey. We offer fundamental to advanced level training, with on-demand, live, and virtual options to suit your busy schedule. [Certifications](https://cloud.google.com/certification/) help you validate and prove your skill and expertise in Google Cloud technologies.

**Manual Last Updated December 10, 2025**

**Lab Last Tested September 15, 2025**

Copyright 2026 Google LLC. All rights reserved. Google and the Google logo are trademarks of Google LLC. All other company and product names may be trademarks of the respective companies with which they are associated.
