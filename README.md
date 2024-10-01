# Welcome to the '365 Free Domain' Subdomain Registry

![image](image/logo.gif)

Welcome to the "365 Free Domain" subdomain registration platform, a platform created for individuals and non-profit organizations and projects.

## Features

### No cost operation
The "365 Free Domain" registry specifically supports non-profits and individuals.

### Easy Verification
Our verification process is simple and straightforward. We rely on your Linux Do account for verification.

### Free Renewal, Forever
Once your subdomain is approved, you will have the right to use it for 1 year without any renewal fees.

<!-- ### Included in Mozilla PSL
Our domain is part of the [Mozilla Public Suffix List (PSL)](https://publicsuffix.org), which enhances security by ensuring subdomains are treated independently by browsers, much like `.co.uk`. However, please note that `.ngo.us` is **not** an ICANN-accredited TLD. See the disclaimer below for more details. -->

## Eligibility Requirements

- **Nonprofits**: Any existing nonprofit organization, project, or program is eligible. It does not need to be incorporated or formally registered with a government agency.
- **Individuals**: You must have a Linux Do account to apply.
- **Legal and bona fide**: The domain you apply for must meet the requirements set forth in our Terms of Service, including being legal and operating in good faith.

## Application Process

### 1. Star and Fork this Repository
Star and [fork this repository](https://github.com/xxecy-114514/365-Free-Domain/fork) to begin the application process.

### 2. Edit Zone File according to your needs
Follow the example format provided to request a domain name. For example, if you wish to request a domain name called "happycat.3656666.xyz" (or "happycat.forks.my.id"), and the name servers are "example1.ns.cloudflare.com." and "example2.ns.cloudflare.com.", edit the zone file "db.3656666.xyz" (or "db.forks.my.id") in your forked repository and add the following block:

```
; (Example) [Your Linux Do account name]
; Submitted by PAUSE [Your Linux Do account name] <LinuxDo@Example.com,https://linux.do/u/[Example]/summary>
Example	86400   IN	NS	Example1.ns.cloudflare.com.
Example	86400	  IN	NS	Example2.ns.cloudflare.com.

```

**Key points to comply:**

1. You need **two comment lines** at the top of your block:
- The first line should be your Linux Do account name.
- The second line should be your Linux Do contact email (to prevent abuse, we only support certain mail providers, please [see](https://github.com/xxecy-114514/365-Free-Domain/blob/main/mail_while_list)). Make sure the domain name of the email address is **not** the same as the '365 Free Domain' you applied for.

2. **Format and order**:
- Make sure the domain name block is in alphabetical order of your Linux Do account name.
- If you apply for multiple domains under the same organization, please list them in alphabetical order.

3. **Name Server (NS) Records**:
- You must include **at least two name servers (NS)** for each domain name.
- Use a Time to Live (TTL) value of `86400` (24 hours).

Once you've finished editing, follow the remaining steps outlined in the PR template to commit, push, and create your pull request. Make sure all entries follow the correct alphabetical order to ensure smooth processing.

### 3. Submit a Pull Request (PR)
Commit and push your changes to your forked repository, then create a pull request (PR) to this repository.

In the body of your PR, provide the following information:

- **Intended use of the domain name**: Describe in detail how you plan to use the domain name.
- **Organization online presence URLs for verification (nonprofits only)**: Include URLs to your organization's public online profiles (e.g., social media accounts) that provide verifiable information about your cause.
- Make sure the exact domain name you are applying for is prominently displayed in one of your profiles (nonprofits only) (e.g., in your bio, a post, or a comment on your organization's social media profile page). For example, if you are applying for "happycat.3656666.xyz", make sure "happycat.3656666.xyz" is visible on your organization's social media.

### 4. Monitor Your PR
After submitting a pull request, please wait for a volunteer to review it (please note that there is only one volunteer (xxecy-114514) and the PR review will not exceed 1 month). PRs that do not pass the check will be ignored. Monitor PRs for any change requests, such as correcting syntax errors in zone files.

After the PR is reviewed and merged, please wait up to 48 hours for the changes to propagate.

## Modify Existing Registry Records

If you need to update or modify the DNS records for an existing '365 Free Domain Name', follow these steps:

1. **Fork the repository**:
Use the same GitHub account that you used to initially register your domain name. Fork this repository if you haven't already, or pull the latest changes from the main repository into your existing fork.

2. **Edit the zone file as needed**:
In your forked repository, make the necessary changes to your domain name's DNS records in the 'db.3656666.xyz' (or 'db.forks.my.id') zone file. Make sure any changes follow the correct format, including using the correct TTL values ​​and name servers.

3. **Commit changes**:
- Make sure your commit is **signed**. If you have set up GPG signing on your GitHub account, you can do this with `git commit -S`.
- In the commit message, clearly describe the changes you made (e.g., "Updated NS records for happycat.3656666.xyz").

4. **Submit a new pull request (PR)**:
Push your changes to your branch and create a new pull request in the main repository. Be sure to provide all relevant details in the PR description, just as you did when you originally requested it.

5. **Monitor and review**:
Make sure all checks pass, and keep an eye on the PR for any changes or update requests from volunteers. Once approved, the changes will be merged and your update will be propagated within 48 hours.


Thank you for choosing '365 Free Domain'
