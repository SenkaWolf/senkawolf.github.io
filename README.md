# Senka's Repo
IOS Jailbreak repo with tweaks I have made

Add to cydia at the url below:
https://senkawolf.github.io/

## Tweaks included in this repo

___
### Senka's Zeppelin Icon Pack
> Icon pack for popular iOS Jailbreak tweak, Zeppelin. Requires jailbroken device and the jailbreak application, Zeppelin.

> **Previews**

![Wolf Preview](https://github.com/SenkaWolf/senkawolf.github.io/blob/master/Screenshots/wolf.png?raw=true){:target="_blank"}
![Senka Preview](https://github.com/SenkaWolf/senkawolf.github.io/blob/master/Screenshots/senka.png?raw=true){:target="_blank"}
![JapChar Preview](https://github.com/SenkaWolf/senkawolf.github.io/blob/master/Screenshots/JapChar.png?raw=true){:target="_blank"}
___
### WTLVTC Zeppelin Icon Pack
> Icon pack for popular iOS Jailbreak tweak, Zeppelin. Requires jailbroken device and the jailbreak application, Zeppelin.

> **Previews**

![WTLogo Preview](https://github.com/SenkaWolf/senkawolf.github.io/blob/master/Screenshots/WTLLogo.png?raw=true){:target="_blank"}
___
### Malipo Sounds Pack
> Sound pack for popular iOS Jailbreak tweak, Malipo. Requires jailbroken device and the jailbreak application, Malipo. This tweak allows custom sounds to play when your device is put on charge.

The list of added sounds are below:
* [Hey Thats Pretty Good](https://youtu.be/nKV1RIX-o1k){:target="_blank"}
* [Damn Son whered You Find This](https://youtu.be/z8RkR4rd7dM){:target="_blank"}
* [HOT HOT HOT](https://youtu.be/vFrNxJoB768){:target="_blank"}
___

showdown.extension('targetlink', function() {
  return [{
    type: 'lang',
    regex: /\[((?:\[[^\]]*]|[^\[\]])*)]\([ \t]*<?(.*?(?:\(.*?\).*?)?)>?[ \t]*((['"])(.*?)\4[ \t]*)?\)\{\:target=(["'])(.*)\6}/g,
    replace: function(wholematch, linkText, url, a, b, title, c, target) {

      var result = '<a href="' + url + '"';

      if (typeof title != 'undefined' && title !== '' && title !== null) {
        title = title.replace(/"/g, '&quot;');
        title = showdown.helper.escapeCharacters(title, '*_', false);
        result += ' title="' + title + '"';
      }

      if (typeof target != 'undefined' && target !== '' && target !== null) {
        result += ' target="' + target + '"';
      }

      result += '>' + linkText + '</a>';
      return result;
    }
  }];
});
