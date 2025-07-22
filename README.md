# Simple Privacy Redirect

<img width="1920" height="1080" alt="privacy-redirect-plus-image" src="https://github.com/user-attachments/assets/2267a677-5dc5-4fa1-aa34-9ffe3f5ad8e6" />


## What this browser extension does
- Redirects requests of various platforms to their privacy-focused alternative frontends.
  
- Does not include any client-side script.

- Uses regex-based declarative rulesets and browser permissions to function.

# Supported Platforms

|Service|Proxy Frontend|Instance Used|Enabled|
|:---:|:---:|:---:|:---:|
|Reddit|Redlib|`redlib.perennialte.ch`|`True`|
|X|Nitter|`nitter.net`|`True`|
|Youtube|Invidious|`inv.nadeko.net`|`True`|
  
## F.A.Q

**Q:** How do I disable redirects for specific platforms?

**A:** Redirects can be disabled by removing site access for related domains in the extensions details page.

## Notes

This project was originally forked from [Old Reddit Redirect](https://github.com/tom-james-watson/old-reddit-redirect).

Find any bugs, problems or have any suggestions? Please feel free to submit an issue or start a discussion.
