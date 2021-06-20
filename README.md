# aimp_custom_component
Custom component for Home Assistant to controling AIMP through network

# screenshot
![screenshot](https://github.com/xilense/aimp_custom_component/raw/master/res/Screenshot01.png)
![screenshot](https://github.com/xilense/aimp_custom_component/raw/master/res/Screenshot02.png)
![screenshot](https://github.com/xilense/aimp_custom_component/raw/master/res/Screenshot03.png)

# dependencies
install needed component
* [AIMP Media Player](http://www.aimp.ru/)
* [Control Plugin Code](https://github.com/a0ivanov/aimp-control-plugin)
* [Alternative Web Interface](https://github.com/gilleswaeber/aimp-web) for Control Plugin

_make sure add firewall exception to AIMP, so Home Assistant can send request & get response through network_

# manual installation
1. Using the tool of choice open the directory (folder) for your HA configuration (where you find `configuration.yaml`).
2. If you do not have a `custom_component` directory (folder) there, you need to create it.
3. In the `custom_components` directory (folder) create a new folder called `aimp`.
4. Download [\_\_init__.py](https://github.com/xilense/aimp_custom_component/blob/master/__init__.py), [manifest.json](https://github.com/xilense/aimp_custom_component/blob/master/manifest.json), [media_player.py](https://github.com/xilense/aimp_custom_component/blob/master/media_player.py) in this repository.
5. Place the files you downloaded in the new directory (folder) you created.
6. Add aimp to media_player config and Restart Home Assistant.

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