# 📊 Adding New Interactive Charts to Your Repository
This guide explains how to add new interactive Plotly dashboards to your existing GitHub Pages repository     <span style="color:blue;">**[[Hyperlink](https://jared-d-sharp.github.io/Tx-Ops-Interactive-Charts/)]**</span>

## 🚀 Step-by-Step Instructions

### Step 1: Navigate to Your Repository
1. Go to **github.com** and sign in to your account
2. Click on your repository name (e.g., "plotly-dashboards") to open it

### Step 2: Create a New Dashboard Folder and File
1. Click the **"Add file"** button near the top of the page
2. Select **"Create new file"** from the dropdown menu
3. In the **"Name your file..."** text box, type: `dashboard-name/index.html`
   - Replace `dashboard-name` with a descriptive name (use hyphens instead of spaces, lowercase letters)
   - Examples: `sales-analysis/index.html`, `customer-metrics/index.html`, `quarterly-report/index.html`
   - The forward slash `/` automatically creates a folder

### Step 3: Add Your Dashboard HTML Content
1. Drag and drop the Plotly dashboard HTML file on your computer into the the large white text area on the GitHub browser page

### Step 4: Commit the New Dashboard File
1. Click the **"Commit changes..."** button
2. A popup window will appear
3. In the **"Commit message"** text box, type: `Add [dashboard name] dashboard`
4. Make sure **"Commit directly to the main branch"** is selected
5. Click the green **"Commit changes"** button

### Step 5: Update the Landing Page
1. Click on your **repository name** at the top-left to go back to the main page
2. Click on the **`index.html`** file to open it
3. Click the **pencil icon** (Edit button) in the top-right corner
4. Find this section:
5. Add a new line before the closing </ul> tag with your new dashboard link:

```
text
<ul class="dashboard-list">
    <li><a href="inhbe-dio/">INHBE DIO Interactive Dashboard</a></li>
    <li><a href="dashboard-name/">Your Dashboard Title</a></li>
</ul>
```

Replace\ 
• dashboard-name with the exact folder name you created in Step 2\
• Your Dashboard Title with a descriptive, user-friendly title for display\

```
text
<ul class="dashboard-list">
    <li><a href="inhbe-dio/">INHBE DIO Interactive Dashboard</a></li>
    <li><a href="sales-analysis/">Q4 2025 Sales Analysis</a></li>
</ul>
```

### Step 6: Commit the Landing Page Update
1. Click "Commit changes..."
2. In the popup, type: Add link to new dashboard
3. Make sure "Commit directly to the main branch" is selected
4. Click the green "Commit changes" button

### Step 7: Access Your New Dashboard
1. Wait 2-3 minutes for GitHub Pages to rebuild your site
• Your new dashboard will be at: https://yourusername.github.io/repository-name/dashboard-name/\
• Your landing page is at: https://yourusername.github.io/repository-name/\

## 📁 Repository Structure
text\
repository-name/\
├── index.html                    (landing page with links)\
├── inhbe-dio/\
│   └── index.html               (INHBE DIO dashboard)\
├── sales-analysis/\
│   └── index.html               (sales dashboard)\
└── customer-metrics/\
    └── index.html               (customer dashboard)\


# 💡 Best Practices

## Naming Conventions:
✅ Use lowercase: sales-report\
✅ Use hyphens: q4-metrics\
✅ Be descriptive: customer-churn-analysis\
✅ Keep short: 2-4 words max\
❌ No spaces: sales report\
❌ No uppercase: Sales-Report\
❌ No underscores: sales_report\

## File Naming:
• Always name dashboard files index.html (lowercase)\
• Creates clean URLs: /sales-dashboard/ instead of /sales-dashboard.html\

## 🔧 Troubleshooting
• 404 Error When Accessing Dashboard:\
• Wait 5-10 minutes for GitHub Pages to rebuild\
• Verify file is named index.html (lowercase)\
• Check folder structure matches URL exactly\
• Ensure repository is Public\
• Clear browser cache or use incognito mode\
• Hard refresh: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)\
• Link on Landing Page Doesn't Work:\
• Verify href matches folder name exactly (case-sensitive)\
• Include trailing slash: href="folder-name/" not href="folder-name"\
• Check for typos in folder name and link\
• Ensure dashboard folder exists in repository\
• Changes Not Showing Up:\
• Wait 2-3 minutes for automatic rebuild\
• Check deployment status in Actions tab (look for green checkmark)\
• Hard refresh: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)\
• Try incognito/private browsing mode\
• Verify changes were committed (check file on GitHub)\

## 🔍 Checking Deployment Status
### Method 1: Actions Tab
• Click "Actions" tab at top of repository\
• Look for "pages build and deployment" workflow\
• Check status:\
🟡 Yellow circle = Building (wait)\
✅ Green checkmark = Deployed\
❌ Red X = Failed (click for details)\

### Method 2: Deployments Section
• Look for "Deployments" in right sidebar of repository main page\
• Click "github-pages"\
• View deployment history\
• Click "View deployment" to visit live site\

## ✅ Quick Checklist
• Created new folder: dashboard-name/index.html\
• Used lowercase letters and hyphens\
• Pasted complete HTML content\
• Committed dashboard file\
• Opened index.html on repository\
• Added link in \<ul class="dashboard-list"> section\
• Link href matches folder name with trailing slash\
• Link text is descriptive\
• Committed landing page changes\
• Waited 2-3 minutes\
• Tested dashboard URL\
• Verified link from landing page\
