## Firefox user.js profiles


### betterdefaults
--- 
This user.js, is the profile Ive used for a long time, and its proven to work, but eventually, I wanted something more than this.
Its based off of the recommendations of [Privacytools.io's about:config](https://privacytools.io/browsers/#about_config).

The goal of this profile, is as following;

- Just work.
- Convinient, yet more secure/private than default configs
- Should work fine for the everyday man, looking for more privacy without comprimising on usablity
- Minimal to no breakage on sites (I personally dont care too much about some breakage, as far as sites functionallity is still kept)

What currently doesnt works;
- [x] Nothing *(afaik anyway)*. Everything should work as expected.

* Ive changed a couple of other things outside of ptio's recommendations;
	* pocket, firefox accounts, extension recommendation, and whatsnew pages is disabled, as I just find them annoying. refer to user.js if you need these.
	* I enabled backspace to go back.
	* Set dom.event.contextmenu.enabled to false. some websites likes to restrict you on rightclicking, and Im not having it, so I changed this setting.
---

### Hardened 
--- 
In this user.js, Ive used [Arkenfox's templated](github.com/arkenfox/user.js), and really just commented/uncommented it to suit my preferences. this setup may or may not work for you, so please dont get worked up if something doesnt work like youre used to, as my preferences may differ from yours. Some breakage is to be expected.

#### Things of interest:
##### Just a small list if things that may be of interest if works, or how it works, and how to *fix* them

- [x] Reddit (partially)

* ~~There seems to be an issue with the logging in part, Im able to enter my credentials, but the redirect dont seem to work as intended~~ old.reddit.com works.
* You should check out [Libreddit](https://github.com/spikecodes/libreddit) instead, for viewing reddit without giving away your IP address.

- [x] ~~YouTube~~ **Invidious**

	* due to **svg.disabled** is set to true, yt player *may* break, if you are for whatever reason still choosing to use youtube, instead of invidious, you may wish to set **svg.disabled** to false. 
		* I havent verified if this actually breaks yt player or not, as I dont use it.
	* You should not use YT anyway, stick with [Invidious](https://github.com/iv-org/invidious).
	* If youre on Android, consider checking out [NewPipe](https://github.com/TeamNewPipe/NewPipe)


- [x] Github (With a quirk)
	* I cant seem to login from github.com's main page, so to login, I have to go straight to [github's login page](www.github.com/login)

* **This profile has some quirks, that may not be what youre used to:**
	* You cannot search directly from the URL bar - this is to prevent leaks, and search engine getting your misspelled queries. To search, either first type @ddg (or any other, check your settings for search engines, and make your own tags to suit your needs), or enable the separate search bar on the side. this is effectivly just a habbit that needs to be unlearned to not find this annoying. if this feature is an aboslute must to have, set **keyword.enabled** to true. see user.js for more info.
	* **privacy.resistFingerprinting.letterboxing** is set to true, which means youll have a white *frame* inside the window, wrapping the website. if your find this to be too annoying, set it to false. Just bear in mind that this is effectivly fingerprintable. for more details, see the user.js file. 

---

#### Addons that might be of interest

* [uBlock Origin](https://github.com/gorhill/uBlock)
	* Convinient scriptblocking tool, with blocklists, which means it can easily be used in the background, or you can run it in advanced mode to block all scripts by default. 

* [Noscript](https://addons.mozilla.org/en-US/firefox/addon/noscript/) - [Website](https://noscript.net/) 
	* Scriptblocking tool, used by Tor Browser. Has alot of good features.
 

* [ClearURLS](https://addons.mozilla.org/en-US/firefox/addon/clearurls/)
	* Blocks trackers on urls, and can clean urls you share.


* [Invidition](https://addons.mozilla.org/en-US/firefox/addon/invidition/)

	* Redirecting tool for youtube -> invidious, and twitter -> nitter.

	* [Privacy-redirect](https://github.com/SimonBrazell/privacy-redirect), an alternative to Invidition, with more redirects.


#### References, links etc
[Privacytools.io](privacytools.io) \
[Arkenfox github](https://github.com/arkenfox/user.js/) \
[R/privacy](https://libredd.it/r/privacy/) \
[R/privacytoolsIO](https://libredd.it/r/privacytoolsIO/) \
[Invidious - Youtube front-end alternative](https://github.com/iv-org/invidious) \
[Techlore - Invidious link](https://invidious.snopyta.org/channel/UCs6KfncB4OV6Vug4o_bzijg) -  [Youtube link](https://www.youtube.com/channel/UCs6KfncB4OV6Vug4o_bzijg) \
[The hated one - Invidious link](https://invidious.snopyta.org/channel/UCjr2bPAyPV7t35MvcgT3W8Q) - [Youtube link](https://www.youtube.com/channel/UCjr2bPAyPV7t35MvcgT3W8Q) \
[EFF - Electronic Frontier Foundation](https://www.eff.org/) \

Related, if you want anonymity and not just privacy:

[Tor Browser](torproject.org) \
[Whonix - basiclly Tor in virtualmachines](whonix.org) \
[Tails OS - Amnesic live USB OS](https://tails.boum.org/)
