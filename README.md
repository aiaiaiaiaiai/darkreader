<p align="center"><a href="https://darkreader.org" target="_blank" rel="noreferrer noopener"><img width="250" alt="Dark Reader's mascot" src="https://raw.githubusercontent.com/darkreader/darkreader.github.io/master/images/darkreader-mascot.svg"></a></p>
<p align="center">Dark Reader <strong>analyzes</strong> web pages and aims to <strong>reduce the eyestrain</strong> while you browse the web.</p>
<br/>
<p align="center"><a rel="noreferrer noopener" href="https://chrome.google.com/webstore/detail/dark-reader/eimadpbcbfnmbkopoojfekhnkhdbieeh/">Chrome Web Store</a> | <a rel="noreferrer noopener" href="https://addons.mozilla.org/en-US/firefox/addon/darkreader/">Firefox Add-ons</a> | <a rel="noreferrer noopener" href="https://microsoftedge.microsoft.com/addons/detail/dark-reader/ifoakfbpdcdoeenechcleahebpibofpc/">Edge Addons</a>
    
<h2 align="center">Dark Reader</h2>  
<br/>
<p align="center">Dark Reader is an <strong>open-source</strong> MIT-licensed <strong>browser extension</strong>, that is designed to analyzes web pages. Based on its analysis Dark Reader will generate a dark mode based on the analysis. Hereby Dark Reader aims to <strong>reduce the eyestrain</strong> of the user. Dark Reader is <strong>feature-rich</strong> and can be configured in many ways trough the UI.</p>

<br/>
<br/>
<h2>Questions</h2>

Most questions can be answered by reading the [help page](https://darkreader.org/help/).
If the help page doesn't answer your question, open up a [issue](https://github.com/darkreader/darkreader/issues/new/) and choose the template 'Question' and fill out the necessary info. 

<h2>How to contribute</h2>

Read more about contributing to Dark Reader in [CONTRIBUTE.md](https://github.com/darkreader/darkreader/blob/master/CONTRIBUTE.md).

<h2>Building for use</h2>

You can install the extension from a file.  
Install [Node.js LTS](https://nodejs.org/en/). Download the source code (or check out from git).  
Open the terminal in the root folder and execute the following commands:  
- `npm install`  
- `npm run release`  

This will generate a `build.zip` file that is useable in a Chromium-based browser and aswell a `build-firefox.xpi` file that is useable in Firefox.

<h2>Using Dark Reader for a website</h2>

You can use Dark Reader to enable dark mode on your website!
- Install the package from NPM (`npm install darkreader`)
- or build from the source code (`npm run api`)
- or include the script via a CDN such as [unpkg](https://unpkg.com/darkreader/) or [jsDelivr](https://www.jsdelivr.com/package/npm/darkreader)

Then you can use the following code to control Dark Reader's API
```javascript
DarkReader.enable({
    brightness: 100,
    contrast: 90,
    sepia: 10
});

DarkReader.disable();

// Enable when system color scheme is dark.
DarkReader.auto({
    brightness: 100,
    contrast: 90,
    sepia: 10
});

// Stop watching for system color scheme.
DarkReader.auto(false);

// Get the generated CSS of Dark Reader returned as a string.
const CSS = await DarkReader.exportGeneratedCSS();
```
... or if you are using ES modules
```javascript
import {
    enable as enableDarkMode,
    disable as disableDarkMode,
    auto as followSystemColorScheme,
    exportGeneratedCSS as collectCSS,
} from 'darkreader';

enableDarkMode({
    brightness: 100,
    contrast: 90,
    sepia: 10,
});

disableDarkMode();

followSystemColorScheme();

const CSS = await collectCSS();
```

<h2>Site fixes</h2>

Automatically syncing the site fixes to every Dark Reader user was disabled because the GitHub team doesn't allow using GitHub as a CDN. Storing these files and making requests to other resources would be expensive and look suspicious. As such, changes are included with each new Dark Reader release.

However, this can be bypassed by the following steps:

- Click Dark Reader icon.
- Click Dev tools (in the bottom-right corner).
- Click Preview new design.
- Enable the `Synchronize site fixes` setting, under `Settings -> Manage Settings`.

<h2 align="center">Contributors</h2>
<br/>
<h3 align="center" color="D66853"><strong>Dark Reader exists thanks to all the people who have contributed to Dark Reader!</strong></h3>
<br/>
<br/>
<p align="center"><a rel="noreferrer noopener" href="https://github.com/darkreader/darkreader/graphs/contributors/"><img src="https://opencollective.com/darkreader/contributors.svg?width=890&button=false" /></a></p>

<h2 align="center">Backers</h2>
<br/>
<h3 align="center" color="D66853"><strong>Thank you to all our generous backers!</strong></h3>
<br/>
<br/>
<p align="center"><a rel="noreferrer noopener" href="https://opencollective.com/darkreader#backers" target="_blank"><img src="https://opencollective.com/darkreader/backers.svg?width=890"></a></p>

<h2 align="center">Sponsers</h2>  
<p align="center">Support Dark Reader by <a rel="noreferrer noopener" href="https://opencollective.com/darkreader#sponsor">becoming a sponsor</a></p>
<h3 align="center" color="D66853"><strong>Thank you to our wonderful sponsors!</strong></h3>

<a href="https://opencollective.com/darkreader/sponsor/0/website" target="_blank" rel="noreferrer noopener"><img src="https://opencollective.com/darkreader/sponsor/0/avatar.svg"></a>
<a href="https://opencollective.com/darkreader/sponsor/1/website" target="_blank" rel="noreferrer noopener"><img src="https://opencollective.com/darkreader/sponsor/1/avatar.svg"></a>
<a href="https://opencollective.com/darkreader/sponsor/2/website" target="_blank" rel="noreferrer noopener"><img src="https://opencollective.com/darkreader/sponsor/2/avatar.svg"></a>
<a href="https://opencollective.com/darkreader/sponsor/3/website" target="_blank" rel="noreferrer noopener"><img src="https://opencollective.com/darkreader/sponsor/3/avatar.svg"></a>
<a href="https://opencollective.com/darkreader/sponsor/4/website" target="_blank" rel="noreferrer noopener"><img src="https://opencollective.com/darkreader/sponsor/4/avatar.svg"></a>
<a href="https://opencollective.com/darkreader/sponsor/5/website" target="_blank" rel="noreferrer noopener"><img src="https://opencollective.com/darkreader/sponsor/5/avatar.svg"></a>
<a href="https://opencollective.com/darkreader/sponsor/6/website" target="_blank" rel="noreferrer noopener"><img src="https://opencollective.com/darkreader/sponsor/6/avatar.svg"></a>
<a href="https://opencollective.com/darkreader/sponsor/7/website" target="_blank" rel="noreferrer noopener"><img src="https://opencollective.com/darkreader/sponsor/7/avatar.svg"></a>
<a href="https://opencollective.com/darkreader/sponsor/8/website" target="_blank" rel="noreferrer noopener"><img src="https://opencollective.com/darkreader/sponsor/8/avatar.svg"></a>
<a href="https://opencollective.com/darkreader/sponsor/9/website" target="_blank" rel="noreferrer noopener"><img src="https://opencollective.com/darkreader/sponsor/9/avatar.svg"></a>
