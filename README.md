# Simple Privacy Redirect

<img width="1920" height="1080" alt="privacy-redirect-plus-image" src="https://github.com/user-attachments/assets/2267a677-5dc5-4fa1-aa34-9ffe3f5ad8e6" />

## What this browser extension does
- Redirects requests of various platforms to their privacy-focused alternative frontends.
  
- Does not include any client-side script to keep it minimally invasive.

- Uses regex-based declarative rulesets and browser permissions to function.

# Supported Platforms

|Platform|Domains Redirected|Paths Redirected|Proxy Frontend|Instance Used|Enabled|
|:---:|:---:|:---:|:---:|:---:|:---:|
|<a href="https://medium.com" target="_blank"><img width="32" height="32" alt="Medium-Icon-White" src="https://github.com/user-attachments/assets/051d2f45-54ff-4706-8af4-06b3a871b43a" /></a>|`medium.com`|`*`|Scribe|`scribe.rip`|`True`|
|<a href="https://www.reddit.com" target="_blank"><img width="32" height="32" alt="Reddit_Icon_FullColor" src="https://github.com/user-attachments/assets/aca193d0-fd46-4f47-ace9-53433b8ff921" /></a>|`www.reddit.com`|`*`|Redlib|`redlib.perennialte.ch`|`True`|
|<a href="https://x.com" target="_blank"><img width="32" height="32" alt="logo-white" src="https://github.com/user-attachments/assets/597c843e-9894-4185-8dcc-6da4fffd1a65" /></a>|`mobile.x.com`, `x.com`, `nitter.net`|`*`, `i/broadcasts/*`|Nitter|`nitter.net`|`True`|
|<a href="https:/www.youtube.com" target="_blank"><img width="32" height="22" alt="YouTube_full-color_icon_(2024) svg" src="https://github.com/user-attachments/assets/96929b09-295d-4d9e-8981-b538cf58249d" /></a>|`m.youtube.com`, `www.youtube.com`|`*`|Invidious|`inv.nadeko.net`|`True`|

# Browser Support

|Browser|Supported|Manifest Version|Install From|Notes|
|:---:|:---:|:---:|:---:|:---:|
|<img width="32" height="32" alt="SmallLogo" src="https://github.com/user-attachments/assets/832e0bdf-8f5b-456a-b07e-6ac565f25367" />|Yes|V3|Coming Soon|
|<img width="32" height="32" alt="SmallLogo" src="https://github.com/user-attachments/assets/88dd6cdd-66ba-4780-9995-e0adf456ebaa" />|Yes|V3|Coming Soon|
|<img width="32" height="32" alt="VisualElements_150" src="https://github.com/user-attachments/assets/a7cb5103-8134-41d7-9169-ab249e837cec" />|Yes|V3|Coming Soon|
|<img width="32" height="32" alt="logo" src="https://github.com/user-attachments/assets/93e694cb-ba43-47e4-8bad-53d9839bd559" />|Yes|V3|Coming Soon|May fail to redirect `youtube.com` but `youtu.be` works|

## F.A.Q

**Q:** How do I disable redirects for specific platforms?

**A:** Redirects can be disabled by removing site access for related domains in the extensions details page.

**Q:** Why don't some redirects work if I click a link that should redirect?

**A:** Some redirects won't work if the site uses client-side navigation as no new network request occurs.

**Q:** Will there be a more expanded version to solve some of the shortfalls of not including client-side script?

**A:** I will make a more dynamic "plus" edition which will use this version as a base but with client-side script for quality-of-life improvements, when I have the time to do so.

## Development

Install [Node and NPM](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm), clone this repo and then run `npm i` in the root directory of the project to install all of the required libraries.

|Command|Description|
|:---:|:---:|
|`npm run build`|Packages necessary assets into a ZIP file.|
|`npm run dev`|Starts a live-reloading development server and opens a targeted browser window for testing.|
|`npm run clean`|Deletes auto-generated/packaged files and folders.|

## Notes

This project was originally forked from [Old Reddit Redirect](https://github.com/tom-james-watson/old-reddit-redirect).

Find any bugs, problems or have any suggestions? Please feel free to submit an issue or start a discussion.
