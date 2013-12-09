# Firefox #  

## Addons ##
*  [Adblock Plus](http://adblockplus.org/en/firefox)  
*  [Element Hiding Helper](http://adblockplus.org/en/elemhidehelper)  
*  [Customizable Shortcuts](https://addons.mozilla.org/en-us/firefox/addon/customizable-shortcuts/)  
Change Meta-k shortcut from Web Search to Home.  
*  [Status-4-Evar](https://addons.mozilla.org/en-US/firefox/addon/status-4-evar/)  
Disable "Show progress in the Location Bar"

        status4evar.progress.urlbar;0
        
*  [FireGestures](https://addons.mozilla.org/en-US/firefox/addon/firegestures/)  
Change Trail Drawing color to red, disable keypress and wheel gestures:

        extensions.firegestures.mousetrail.color;#FF0000  
        extensions.firegestures.keypressgesture;false  
        extensions.firegestures.wheelgesture;false
        
*  [NoScript](http://noscript.net/)  

## Configuration ##

        browser.newtab.url;about:blank
        general.smoothScroll;false
        network.proxy.autoconfig_url;http://www-sul.stanford.edu/apcproxy/suproxy.pac
        network.proxy.type;2

## Fix abnormally-sized go button in urlbar ##
Navigate to `~/Library/Application Support/Firefox/Profiles/XXXXXX.default/chrome/`.
Create `chrome/userChrome.css` (creating folder `chrome` if necessary) with contents:  

        /* The @namespace line must be the first statement in the file */
        @namespace url("http://www.mozilla.org/keymaster/gatekeeper/there.is.only.xul");
        #urlbar-go-button, #go-button { display: none !important }

Restart Firefox.
