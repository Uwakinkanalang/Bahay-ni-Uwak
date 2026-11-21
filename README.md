# Bahay ni Uwak

A responsive bedspace rental management website.

## Features

- Dashboard with renter totals, active rentals, available bedspaces, and upcoming move-outs
- Combined Renters Management workspace: searchable renter list and selected renter profile
- Add, edit, and delete renter records
- Rental calendar showing move-in and move-out dates
- Philippine peso (₱) rent display
- Responsive layout for desktop and mobile

## Run locally

Open `index.html` in a modern browser.

## Publish with GitHub Pages

1. Open the repository's **Settings**.
2. Select **Pages** in the sidebar.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch **main** and folder **/(root)**, then save.
5. Wait for GitHub Pages to publish the site. The Pages URL will appear in that section.

## Important: where renter data is stored

This first version stores records in the browser's local storage. Data remains in the same browser on the same device, but it is **not shared** with other devices or users. Clearing browser data can erase those records. For a live rental operation with shared access, connect a hosted database (such as Supabase or Firebase) and add sign-in and access rules before entering real renter information.

The dashboard currently assumes **10 total bedspaces** when calculating availability. Update the `10` values in `index.html` if your property has a different capacity.
