# Arclog Website

Landing page, Privacy Policy, and Terms & Conditions for [arclog.online](https://arclog.online).

## Setup Instructions

### 1. Create a GitHub Repository
- Go to [github.com/new](https://github.com/new)
- Name it anything (e.g., `arclog-website`)
- Set it to **Public**
- Click **Create repository**

### 2. Upload Files
Upload all files from this folder to the repository:
- `index.html` — Landing page
- `privacy-policy.html` — Privacy Policy
- `terms-and-conditions.html` — Terms & Conditions
- `CNAME` — Custom domain config

### 3. Enable GitHub Pages
- Go to **Settings** → **Pages**
- Under **Source**, select **Deploy from a branch**
- Choose **main** branch and **/ (root)** folder
- Click **Save**

### 4. Configure GoDaddy DNS
Go to your GoDaddy DNS settings for `arclog.online` and set up these records:

| Type  | Name | Value                  |
|-------|------|------------------------|
| A     | @    | 185.199.108.153        |
| A     | @    | 185.199.109.153        |
| A     | @    | 185.199.110.153        |
| A     | @    | 185.199.111.153        |
| CNAME | www  | YOUR_GITHUB_USERNAME.github.io |

> Replace `YOUR_GITHUB_USERNAME` with your actual GitHub username.

### 5. Enable HTTPS
- After DNS propagates (can take up to 48 hours, usually 10-30 minutes)
- Go back to **Settings** → **Pages** in your GitHub repo
- Check **Enforce HTTPS**

### 6. Update Play Store Link
Replace `YOUR_APP_ID` in `index.html` with your actual Google Play package name. 
Search for `YOUR_APP_ID` and replace all 4 occurrences.

---

Your site will be live at **https://arclog.online** 🚀
