## Firefox user.js profiles
In this repo, youll find 3 sets of user.js', to use on your firefox browser (or forks that support it). Beginning from a better default, with privacytools.io's recommendations with more, ending with a really hardened setup made from arkenfox's user.js.



### betterdefaults-user.js
This user.js, is the profile Ive used for a long time, and its proven to work, but eventually, I wanted something more than this.
Its based off of the recommendations of [Privacytools.io's about:config](https://privacytools.io/browsers/#about_config).

The goal of this profile, is as following;

- Just work.
- Convinient, yet more secure/private than default configs
- Should work fine for the everyday man, looking for more privacy without comprimising on usablity
- Minimal breakage on sites (I personally dont care too much about some breakage, as far as sites functionallity is still retained
What currently works;
- [x] Everything *(afaik anyway*)

* Ive changed a couple of other things outside of ptio's recommendations;
	* pocket, firefox accounts, extension recommendation, and whatsnew pages is disabled, as I just find them annoying. refer to user.js if you need these.
	* I enabled backspace to go back.
	* Set dom.event.contextmenu.enabled to false. some websites likes to restrict you on rightclicking, and Im not having it, so I changed this setting.

### Hardened 
In this user.js, Ive used [Arkenfox's templated](github.com/arkenfox/user.js), and really just commented/uncommented it to suit my preferences. this may or may not work for you, so please dont get worked up if something doesnt work like youre used to, as my preferences may differ from yours. Some breakage is to be expected.

#### Things of interest:
##### Just a small list if things that may be of interest if works, or how it works, and how to *fix* them

- [x] Reddit (partially)

* ~~There seems to be an issue with the logging in part, Im able to enter my credentials, but the redirect dont seem to work as intended~~ old.reddit.com works.

- [x] ~~YouTube~~ **Invidious**

- [ ] Github -  Cant seem to access the side menu where you log in. have to use betterdefaults profile to access untill I figure out what setting is tripping it.

* due to **svg.disabled** is set to true, yt player *may* break, if you are for whatever reason still choosing to use youtube, instead of invidious, you may wish to set **svg.disabled** to false. 
* I havent tested youtube.com, ~~nor yt player on invidious,~~ (yt player option on invidious does work for me)  as I dont personally use it.
* You should not use YT anyway, stick with [Invidious](https://github.com/iv-org/invidious).

* **This profile has some quirks, that may not be what youre used to:**
	* You cannot search directly from the URL bar - this is to prevent leaks, and search engine getting your misspelled URLs. to search, either first type @ddg (or any other, check your settings for search engines, and make your own tags to suit your needs), or enable the separate search bar on the side. this is effectivly just a habbit that needs to be unlearned to not find this annoying. if this feature is an aboslute must to have, set **keyword.enabled** to true. see user.js for more info.
	* **privacy.resistFingerprinting.letterboxing** is set to true, which means youll have sort of a white *frame* inside the window, wrapping the website. this may be annoying to you, and if thats the case, set it to false. Just bear in mind that this is effectivly fingerprintable. for more details, see the user.js file. 


### Extra-hardened **(WIP!)**
This profile is as of writing this not started to be worked on.
The file is added in the repo, but its still the same as the hardened user.js, because its based on the same settings, just with some other further hardening to it.



### Other stuff that might be of interest
#### Addons

* [Umatrix](https://github.com/gorhill/uMatrix)
	* **WARNING!! No longer recieving updates!!**
	* Advanced Blocking utilty, that can block scripts, cookies, CSS, images frames..

* [uBlock Origin](https://github.com/gorhill/uBlock)
	* Convinient scriptblocking tool, with blocklists, which means it can easily be used in the background, or you can run it in advanced mode to block all scripts by default. 

* [Noscript](https://addons.mozilla.org/en-US/firefox/addon/noscript/) - [Website](https://noscript.net/) 
	* Scriptblocking tool, used by Tor Browser. Has alot of good features.
 
* *HTTPS everywhere* 
	* **No longer needed with FF https-only mode.** Enabled on all profiles.

* [ClearURLS](https://addons.mozilla.org/en-US/firefox/addon/clearurls/)
	* Blocks trackers on urls, and can clean urls you share.

* [Privacy-redirect](https://github.com/SimonBrazell/privacy-redirect)
		* Redirects Youtube, Twitter, Instagram and more. 
	* [Invidition](https://addons.mozilla.org/en-US/firefox/addon/invidition/)
		* Redirecting tool for youtube -> invidious, and twitter -> nitter,

#### References, links etc
[Privacytools.io](privacytools.io) \
[Arkenfox github](https://github.com/arkenfox/user.js/) \
[R/privacy](reddit.com/r/privacy/) \
[R/privacytoolsIO](reddit.com/r/privacytoolsio) \
[Invidious - Youtube front-end alternative](https://github.com/iv-org/invidious) \
[Techlore - Invidious link](https://invidious.snopyta.org/channel/UCs6KfncB4OV6Vug4o_bzijg) -  [Youtube link](https://www.youtube.com/channel/UCs6KfncB4OV6Vug4o_bzijg) \
[The hated one - Invidious link](https://invidious.snopyta.org/channel/UCjr2bPAyPV7t35MvcgT3W8Q) - [Youtube link](https://www.youtube.com/channel/UCjr2bPAyPV7t35MvcgT3W8Q) \
[EFF - Electronic Frontier Foundation](https://www.eff.org/) \
[Tor Browser](torproject.org) \
[Whonix - basiclly Tor in virtualmachines](whonix.org) \
[Tails OS - Amnesic live USB OS](https://tails.boum.org/) \
