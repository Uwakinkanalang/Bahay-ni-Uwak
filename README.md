# Bahay ni Uwak

A responsive bedspace rental management website for experimenting with renter records.

## Current features

- Dashboard with renter totals, active rentals, available bedspaces, and upcoming move-outs
- Searchable renter list and selected renter profile
- Add, edit, and delete renter records
- Rental calendar showing move-in and move-out dates
- Philippine peso (₱) rent display
- Notes on each renter
- JSON backup export and import
- Responsive desktop and mobile layout

## Run locally

Open `index.html` in a modern browser.

## Publish with GitHub Pages

1. Open the repository's **Settings**.
2. Select **Pages** in the sidebar.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch **main** and folder **/(root)**, then save.
5. Wait for GitHub Pages to publish the site. The Pages URL will appear in that section.

## How testing data storage works

The app currently saves changes in the browser's local storage. To keep a copy in GitHub:

1. Open the website in the browser where you entered your test records.
2. Click **Export JSON**. A dated backup file will be downloaded.
3. In GitHub, open this repository and upload the backup file into a folder such as `backups/`.
4. On another browser or device, download that JSON file from GitHub and use **Import JSON** in the website.

Import replaces the renter list currently stored in that browser, so export a backup first if you need to preserve its current data.

**Important limitations:** This is a manual backup workflow, not live synchronization. GitHub Pages is a static website and cannot safely write to a GitHub repository directly without a secure server-side component. Do not put a GitHub access token in browser JavaScript.

## Privacy warning

Before uploading real renter information, change this repository's visibility to **Private** in GitHub repository Settings → General → Danger Zone → Change repository visibility. A public repository makes uploaded renter records visible to everyone. Keep real renter data private and only grant access to trusted people.

## Bedspace capacity

The dashboard currently assumes **10 total bedspaces** when calculating availability. Update the `10` values in `index.html` if your property has a different capacity.
