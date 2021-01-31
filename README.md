## Firefox user.js profiles
In this repo, youll find two user.js profiles, each have their own usecases.
I rearly if ever use the PTIO one, but its convinient to have one that I know work everywwhere, while yet being more secure/private than default configs.
This repo was initially created with the intention of making it convinient for me, if I were to loose my configs, but I figured, why not make it so others can enjoy it aswell.


### PTIO-user.js
This user.js, is the profile Ive used for a long time, and its proven to work.
Its based off of the recommendations of [Privacytools.io's about:config](https://privacytools.io/browsers/#about_config).
The goal of this profile, is as following;

- Just work.
- Convinient, yet more secure/private than default configs
- Should work fine for the everyday man, looking for more privacy without comprimising on usablity
- Minimal breakage on sites (I personally dont care too much about some breakage, as far as sites functionallity is still retained
What currently works;
- [x] Everything

* Ive changed a couple of other things outside of ptio;
	* pocket, firefox accounts, extension recommendation, and whatsnew pages is disabled, as I just find them annoying. refer to user.js if you need these.
	* I enabled backspace to go back.
	* Set dom.event.contextmenu.enabled to false. some websites likes to restrict you on rightclicking, and Im not having it, so I changed this setting.

### Arkenfox-based
In this user.js, Ive used [Arkenfox's templated](github.com/arkenfox/user.js), and initially just commented/uncommented it to suit my preferences. this may or may not work for you, so please dont get worked up if something doesnt work like youre used to, as my preferences may differ from yours. Below, I also started a list of things that may be of interest to you. 
Ive focused on hardening, but Ive tried not to obliterate usablity to an unsuable state.
I plan on using this as my main profile, so being able to do everyday stuff like i.e. reddit or use ~~youtube~~ *coff*, **invidious** should be expected to work. 
Some breakage is to be expected.

#### Things of interest:
##### Just a small list if things that may be of interest if works, or how it works, and how to *fix* them

- [ ] Reddit (partially)

* ~~There seems to be an issue with the logging in part, Im able to log in, but the screen wont load after this~~ old.reddit.com works.

- [x] ~~YouTube~~ **Invidious**

* due to svg.disabled is set to true, yt player may break, if you for some reason refuse to use invidious, instead of youtube, you may wish to set **svg.disabled** to false instead. 
* I havent tested YT's site, nor yt player on invidious, as I dont personally use it.
* You should not use YT anyway, stick with Invidious.

* This profile has some quirks, that may not be what youre used to:
	* You cannot search directly from the URL bar, this is to prevent leaks, and search engine getting your misspelled URLs. to search, either first type @ddg (or any other, check your settings for searh engines, and make your own tags to suit your needs), or enable the separate search bar on the side. this is effectivly just a habbit that needs to be unlearned to not find this annoying. if this feature is an aboslute must to have, set **keyword.enabled** to true. se user.js for more info.
	* **privacy.resistFingerprinting.letterboxing** is set to true, which means youll have sort of a white *frame* inside the window, wrapping the website. this may be annoying to you, and if thats the case, set it to false. Just bear in mind that this is effectivly fingerprintable. for more details, see the user.js file. 

I will try my best to keep some track of Arkenfox's work, and add/remove stuff as theyre added/removed/depreciated as firefox is updated.

Feel free to use these as you wish, or create an issue if theres any problems that needs to be solved.
