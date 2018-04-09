# Week-7
WordPress Vulnerabilities
# Project 7 - WordPress Pentesting

Time spent: **X** hours spent in total

> Objective: Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. XSS Script Error alert
  - Summary: Creating a user account in WordPress. Using that account to show Xss scripting vulnerability. When the admin logs in and views the site, the xss scripting error will show up. 
    - Vulnerability types: XSS
    - Tested in version: 4.1
    - Fixed in version: 4.1.19
  - GIF Walkthrough: <a href="https://imgur.com/Bg0UP7p"><img src="https://i.imgur.com/Bg0UP7p.gif" title="source: imgur.com" /></a>
  - Steps to recreate: Login to the user that you created. Go to the site and post a comment on the website with the Xss script. The xss script I used was IMG SRC="#" ONERROR="alert('Hacked')". So anytime the page loads an error pops up with "Hacked". 
1. (Required) Vulnerability Name or ID
  - Summary: Showing a xss scripting error for when your mouse goes over a link or something in the site. Just shows that there are vulnerabilities within the site.
    - Vulnerability types: XSS onmouseover error
    - Tested in version: 4.1
    - Fixed in version: 4.1.19
  - GIF Walkthrough: <a href="https://imgur.com/lczgS4h"><img src="https://i.imgur.com/lczgS4h.gif" title="source: imgur.com" /></a>
  - Steps to recreate: Log into the user you created. Go to the wpdistillery site, post a comment and use the xss script <b onmouseover=alert('Hacked!')>click me!</b>. When the admin user logs in and sees this, when he roles the mouse over the "click me!" it'll pop up an error "Hacked". 
1. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)


## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work
