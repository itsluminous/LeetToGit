
# LeetToGit - Sync your code with GitHub

<p align="center">
  <a href="https://github.com/itsluminous/LeetToGit/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="license"/>
  </a>
  <a href="https://github.com/itsluminous/LeetToGit/graphs/contributors" alt="Contributors">
    <img src="https://img.shields.io/github/contributors/itsluminous/LeetToGit" />
  </a>
</p>
<h1 align="center">
    <img src="assets/octocode.png" alt="LeetToGit" width="400">
</h1>


## What is LeetToGit?

A chrome extension that automatically pushes your code to GitHub when you pass all tests on a <a href="http://leetcode.com/">Leetcode</a> problem.


## Why LeetToGit?

There's no easy way of accessing your leetcode problems in one place! Moreover, pushing code manually to GitHub from Leetcode is very time consuming. So, why not just automate it entirely without spending a SINGLE additional second on it?

## Screenshot

<h1 align="center">
    <img src="assets/extension/2.png" alt="leetcode view" width="800">
</h1>

## Supported UI

LeetToGit works with two different Leetcode UIs. There are known issues when using the plugin with the "non-dynamic layout". Please use one of the following:

1. **old layout** or
2. new **"dynamic layout"**

## Limitations

Your submission may not be successfully uploaded to GitHub if you update the text in the editor too fast. It is necessary to wait for 4 seconds (until the spinner stops) after submitting the solution before entering new characters, switching languages, or switching editors. During this period, your solution is being pushed to GitHub, and the website should maintain its layout without alteration. While this process is less than ideal, we have not found a better solution so far. Sorry for this inconvenience! If you find a fix, your PRs are welcome!







## Installation

Please follow the steps below.

* Create your own OAuth app in GitHub (https://github.com/settings/applications/new) and store CLIENT_ID and CLIENT_SECRET confidentially
    * Application name: [CUSTOM]
    * Homepage URL: https://github.com/itsluminous/LeetToGit
    * Authorization callback URL: https://github.com/
* Download the project ZIP (<a href="https://github.com/itsluminous/LeetToGit/releases">Releases</a>) or clone this repository
* Run ```npm run setup``` to install the developer dependencies
* Update CLIENT_ID and CLIENT_SECRET in ```scripts/authorize.js``` and ```scripts/oauth2.js``` with your ids
* Go to <a href="chrome://extensions">chrome://extensions</a>
* Enable <a href="https://www.mstoic.com/enable-developer-mode-in-chrome/">Developer mode</a> by toggling the switch on top right corner
* Click **"Load unpacked"**
* Select the entire LeetToGit folder


## Setup

1. After installing the LeetToGit, launch the plugin
2. Click on **"Authorize with GitHub"** to set up your account with LeetToGit
3. Setup an existing/new repository with LeetToGit (private by default) by clicking **"Get Started"**
4. Begin Leetcoding! To view your progress, simply click on the extension!


## Supported npm commands

```bash
npm run               # Show available commands
npm run setup         # Install dependencies
npm run format        # Auto-format JavaScript, HTML/CSS
npm run format-test   # Test if code is formatted properly
npm run lint          # Lint JavaScript
npm run lint-test     # Test if code is linted properly
```

## Contribution

Please help to further improve this awesome plugin! We would appreciate your support. Your pull requests are welcome!

Don't forget to star this repository for further development of new features.

