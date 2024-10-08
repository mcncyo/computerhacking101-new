---
title: How to Set Up a Secure GitHub Account and Use Security Features
url: "/tutorial/github/createingSecureGithubAccount"
date: 2022-03-08T12:54:29
lastmod: 2023-02-22T19:54:29
#image: images/syncthingonlinux/installsyncthingonlinux.png
author: Chris Allen
categories:
- github
- git

description: Learn how to secure your GitHub account and protect your data with strong passwords, two-factor authentication, SSH keys, app review, permissions, and security advisories. Keep your GitHub safe with these tips.
---


GitHub is a popular platform used by developers to collaborate on projects and share code. However, as with any online platform, it's important to take steps to secure your account and protect your data. In this guide, we'll walk you through the steps you can take to set up a secure GitHub account and use security features.

## Create a Strong Password

When creating your GitHub account, make sure to use a strong password that is not easily guessable. Avoid using common words, phrases, or patterns. Instead, use a combination of letters, numbers, and symbols to create a strong and unique password.

## Enable Two-Factor Authentication (2FA)

Two-factor authentication adds an extra layer of security to your account by requiring you to provide a second form of identification, such as a code sent to your phone or generated by an app, in addition to your password. To enable 2FA on GitHub, follow these steps:

1. Log in to your GitHub account and click on your profile picture in the top-right corner of the page.

2. Click on "Settings" in the dropdown menu.

3. Click on "Security" in the left-hand sidebar.

4. Under "Two-factor authentication," click on "Set up two-factor authentication."

5. Follow the prompts to set up 2FA using either a text message or an authentication app.

## Set Up SSH Keys

SSH keys allow you to securely authenticate with GitHub without having to enter your username and password every time you push or pull code. To set up SSH keys on GitHub, follow these steps:

Generate an SSH key pair on your local machine using the following command in your terminal:

``` bash
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

When prompted, save the key pair to the default location by pressing "Enter."
Add the SSH key to your GitHub account by following these steps:

1. Log in to your GitHub account and click on your profile picture in the top-right corner of the page.
2. Click on "Settings" in the dropdown menu.
3. Click on "SSH and GPG keys" in the left-hand sidebar.
4. Click on "New SSH key."
5. Give the key a descriptive title and paste the contents of the public key file into the "Key" field.
6. Click "Add SSH key."

Test the SSH key by running the following command in your terminal:

``` bash
    ssh -T git@github.com
```

## Review and Manage Your Authorized Applications

GitHub allows you to authorize third-party applications to access your account, such as continuous integration services or code analysis tools. It's important to regularly review these authorized applications and revoke access for any that you no longer use or trust. To manage your authorized applications on GitHub, follow these steps:

1. Log in to your GitHub account and click on your profile picture in the top-right corner of the page.

2. Click on "Settings" in the dropdown menu.

3. Click on "Applications" in the left-hand sidebar.

4. Review the list of authorized applications and revoke access for any that you no longer use or trust.

## Use Strong Permissions and Access Controls

If you are working on a project with others, make sure to use strong permissions and access controls to restrict access to sensitive information. GitHub offers features like protected branches, pull request reviews, and branch restrictions to help you manage access to your repositories. To set up permissions and access controls on GitHub, follow these steps:

1. Navigate to the repository that you want to set up permissions and access controls for.

2. Click on the "Settings" tab in the top-right corner of the repository page.

3. Click on "Branches" in the left-hand sidebar.

4. Use the dropdown menus to select which users or teams can push to or merge from the branch.

5. Enable pull request reviews by clicking on "Require pull request reviews" and specifying the number of reviewers required.

6. Set up branch restrictions by clicking on "Branch protection rules" and selecting the branch you want to protect. Then, enable the "Require pull request reviews" and "Require status checks" options.

## Stay Up-to-Date on Security Advisories

GitHub regularly publishes security advisories for vulnerabilities that affect its platform. It's important to stay up-to-date on these advisories and take any recommended actions to secure your account and repositories. To view security advisories on GitHub, follow these steps:

Visit the GitHub Security Advisory page at <https://github.com/advisories>.

Review the list of advisories and take any recommended actions to secure your account and repositories.

In conclusion, by following these steps, you can help to ensure that your GitHub account and repositories are secure. By using strong passwords, enabling two-factor authentication, setting up SSH keys, reviewing and managing authorized applications, using strong permissions and access controls, and staying up-to-date on security advisories, you can protect your data and collaborate with others on GitHub with confidence.
