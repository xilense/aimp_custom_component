# aimp_custom_component
Custom component for Home Assistant to controling AIMP through network

# screenshot
![screenshot](https://github.com/xilense/aimp_custom_component/raw/master/aimp/res/Screenshot01.png)
![screenshot](https://github.com/xilense/aimp_custom_component/raw/master/aimp/res/Screenshot02.png)
![screenshot](https://github.com/xilense/aimp_custom_component/raw/master/aimp/res/Screenshot03.png)

# dependencies

install needed component
* [AIMP Media Player](http://www.aimp.ru/)
* [Control Plugin Code](https://github.com/a0ivanov/aimp-control-plugin)
* [Alternative Web Interface](https://github.com/gilleswaeber/aimp-web) for Control Plugin

_make sure add firewall exception to AIMP, so Home Assistant can send request & get response through network_

# yaml config 
```
media_player:
  - platform: aimp
    name: 'AIMP'
    host: !secret aimp_ip
    port: 3333
```

# to-do
* Add browse_media


<a href="https://www.buymeacoffee.com/xilense" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/white_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>