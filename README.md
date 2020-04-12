# APG-TouchBar  
An useful [MTMR (My Touchbar My Rules)](https://mtmr.app) preset for MacBook Pro Touch bar: [gouillou.com/scripts/apg-touchbar.html](http://gouillou.com/scripts/apg-touchbar.html) 

![](https://raw.githubusercontent.com/evopub/APG-TouchBar/master/apg-touchbar.png) 

## Licence 

MIT   
©Philippe Gouillou |  [http://gouillou.com](http://gouillou.com)  

## Versions 

- v.1.0 (12 april 2020): First public version 

## Installation 

This preset is to be used, in complete or in part, with: [My TouchBar My rules. The Touch Bar Customisation App for your MacBook Pro](https://mtmr.app) 

## Buttons 

- Escape  
- Exit (return to default TouchBar)  
- Activate Applications:  
	- Finder  
	- [VS Code](https://code.visualstudio.com/)
	- [The Archive](https://zettelkasten.de/the-archive/)
	- [Pixelmator](https://www.pixelmator.com/)
- Brightness  
	- Brightness Down  
	- Brightness Up  
- Function Keys (Escape or Unescape lines to select):  
	- F5  
	- F6  
	- F9  
	- F10  
- Sound volume:  
	- Silence  
	- Volume Down  
	- Volume Up  
- Yandex Weather  
- Display sleep  
- Time 

## SOURCES: 

- Icons: *DisplaySleep* copied from [@darkomen78](https://github.com/Toxblh/MTMR-presets/blob/master/darkomen78/slg.json), others generated through [base64-image.de](https://www.base64-image.de/)
- AppleScript Key codes: [eastmanreference.com](https://eastmanreference.com/complete-list-of-applescript-key-codes) 

## Code 

```javascript  
  [
    { "type": "escape", "align": "left" },
    { "type": "exitTouchbar", "width": 44, "align": "left"},
  
    { "type": "staticButton", "title": "", "width": 55, "bordered": true, "align": "left", "action": "appleScript", "actionAppleScript": {"inline": "tell application  \"Finder\" to activate"},"image": {"base64": "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" }},
    { "type": "staticButton", "title": "", "width": 55, "bordered": true, "align": "left", "action": "appleScript", "actionAppleScript": {"inline": "tell application \"Visual Studio Code\" to activate" }, "image": {"base64":"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"}},
    { "type": "staticButton", "title": "", "width": 55, "bordered": true, "align": "left", "action": "appleScript", "actionAppleScript": {"inline": "tell application \"The Archive\" to activate" }, "image": { "base64": "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"}},
    { "type": "staticButton", "title": "", "width": 55, "bordered": true, "align": "left", "action": "appleScript", "actionAppleScript": {"inline": "tell application \"Pixelmator\" to activate"}, "image": {"base64": "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"}},
  
    { "type": "brightnessDown", "width": 44, "align": "left" },
    // { "type": "brightness", "width": 100, "align": "left", "image": {"base64":"iVBORw0KGgoAAAANSUhEUgAAAIAAAACAAQMAAAD58POIAAAABGdBTUEAALGPC/xhBQAAAAFzUkdCAK7OHOkAAAAGUExURffLOPfLNyaSVzUAAAACdFJOU/kBxOqnWgAAAbJJREFUSMfVljtyhDAQBVulQCFH4CgcDR1NR9ERFBKoeA5GfGddtkNvwFINFKP5tED22+Zxwviv6QVKfIEc/iNoF5gkpLIeYI8SUp4PsAUJiekADQntF6isQjvxCTrhAJlFqMMBeIH9BMsD7DAb2BhvYbIyNAOCZIWqYKGTpDZJFQu9EKVd44RxQRq3IrULWD62C8wSssWUZEsR0k6wcDOrJZmoBpMKI+s5qkBQCQOUJADVOECdOsDS0gDbsgHMfT4rVwHSrZQFIN5ABka8BgDgAeZ+BztBgvUEnSgVlhNsTFJjvoF5HAZorBpdYKAiSRbqNyBIUr6AjZMdPwO72R40MElS+wZUWA+wQ6LAYkFvdIhkmA+wQSDDdIAGAZ6A34H0x0fca11gBZZsIHSIfnE/5+NjCn/OuiuUB+/aunZwDeNayjXdTpDN0wlY+r1PfWu75nfj8RogN2JuCN2Y5qgMwTI0wGPUnQw6Qarx0sVNKA5Mn6VUL22lIbZoYitDbPmlvocc9Umfl2D7adz1reC3pF8av4m+DCenp/ndZuG3E7fhuC3pH2+vnz8V3MfE+bnxBTXuuIMTrLWHAAAAAElFTkSuQmCC" }},
    { "type": "brightnessUp", "width": 44, "align": "left" },
    
    // { "type": "staticButton", "title": "F1", "action": "keyPress", "keycode": 107, "width": 50, "align": "left"},
    // { "type": "staticButton", "title": "F2", "action": "keyPress", "keycode": 113, "width": 50, "align": "left"},
    // { "type": "staticButton", "title": "F3", "action": "keyPress", "keycode": 160, "width": 50, "align": "left"},
    // { "type": "staticButton", "title": "F4", "action": "keyPress", "keycode": 131, "width": 50, "align": "left"},
    { "type": "staticButton", "title": "F5", "action": "keyPress", "keycode": 96, "width": 50, "align": "left"},
    { "type": "staticButton", "title": "F6", "action": "keyPress", "keycode": 97, "width": 50, "align": "left"},
    // { "type": "staticButton", "title": "F7", "action": "keyPress", "keycode": 98, "width": 50, "align": "left"},
    // { "type": "staticButton", "title": "F8", "action": "keyPress", "keycode": 100, "width": 50, "align": "left"},
    { "type": "staticButton", "title": "F9", "action": "keyPress", "keycode": 101, "width": 50, "align": "left"},
    { "type": "staticButton", "title": "F10", "action": "keyPress", "keycode": 109, "width": 50, "align": "left"},
    // { "type": "staticButton", "title": "F11", "action": "keyPress", "keycode": 103, "width": 50, "align": "left"},
    // { "type": "staticButton", "title": "F12", "action": "keyPress", "keycode": 111, "width": 50, "align": "left"},
  
    { "type": "mute", "width": 40, "align": "right" },
    { "type": "volumeDown", "width": 44, "align": "right" },
    // { "type": "volume", "width": 90, "align": "right" },
    { "type": "volumeUp", "width": 44, "align": "right" },
  
    { "type": "yandexWeather", "icon_type": "images", "units": "metric", "align": "right", "refreshInterval": 300 },
  
    { "type": "displaySleep", "width": 44, "align": "right", "title":"",    "image": {"base64":"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"},},
  
    { "type": "timeButton", "align": "right", "bordered": true  }
  ]   
```