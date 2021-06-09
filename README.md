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

_Make sure add firewall exception to AIMP, so Home Assistant can send request & get response through network_

# yaml config 
```
- platform: aimp
  name: 'AIMP'
  host: !secret aimp_ip
  port: 3333
```

# to-do
* Add seek_media bar progress
* Add browse_media
