# Simple Privacy Redirect

<img width="1920" height="1080" alt="privacy-redirect-plus-image" src="https://github.com/user-attachments/assets/2267a677-5dc5-4fa1-aa34-9ffe3f5ad8e6" />

## What this browser extension does
- Redirects requests of various platforms to their privacy-focused alternative frontends.
  
- Does not include any client-side script to keep it minimally invasive.

- Uses regex-based declarative rulesets and browser permissions to function.

# Supported Platforms

|Service|Proxy Frontend|Instance Used|Enabled|
|:---:|:---:|:---:|:---:|
|Reddit|Redlib|`redlib.perennialte.ch`|`True`|
|X|Nitter|`nitter.net`|`True`|
|Youtube|Invidious|`inv.nadeko.net`|`True`|

# Supported Browsers

|Browser|Supported|
|:---:|:---:|
|Chrome|`True`|
  
## F.A.Q

**Q:** How do I disable redirects for specific platforms?

**A:** Redirects can be disabled by removing site access for related domains in the extensions details page.

**Q:** Why don't some redirects work if I click a link that should redirect?

**A:** Some redirects won't work if the site uses client-side navigation as no new network request occurs.

**Q:** Will there be a more expanded version to solve some of the shortfalls of not including client-side script?

**A:** I will make a more dynamic "plus" edition which will use this version as a base but with client-side script for quality-of-life improvements, when I have the time.

## Development

Install [Node and NPM](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm), clone this repo and then run `npm i` in the root directory of the project to install all of the required libraries.

|Command|Description|
|:---:|:---:|
|`npm run build`|Packages necessary assets into a ZIP file.|
|`npm run dev`|Starts live-reloading development server and opens a targeted browser window for testing.|
|`npm run clean`|Deletes auto-generated/packaged files and folders.|

## Notes

This project was originally forked from [Old Reddit Redirect](https://github.com/tom-james-watson/old-reddit-redirect).

Find any bugs, problems or have any suggestions? Please feel free to submit an issue or start a discussion.
