# Homebridge-airly
[![NPM Version](https://img.shields.io/npm/v/homebridge-airly.svg)](https://www.npmjs.com/package/homebridge-airly)

**Homebridge plugin that is showing information about air quality from Airly API.**

Project is based on [homebridge-weather](https://github.com/werthdavid/homebridge-weather) and [homebridge-arinow](https://github.com/ToddGreenfield/homebridge-airnow).

Currently **Airly** is supporting only Polish localizations.

## 安装
1. 安装 Homebridge 使用: `(sudo) npm install -g --unsafe-perm homebridge`.
1. 安装 这个 插件 使用: `(sudo) npm install -g homebridge-airly`.
1. 获取 **API Key** from Airly. 登陆 <https://developer.airly.eu/login> 生成.
1. Find out your coordinates (latitude and longitude). Based on that information Airly will show measurements from nearest sensor. You can use this page <https://www.latlong.net/>.
1. 更新你的配置文件

This plugin is returning data such as: AQI (Air Quality Index), PM2.5, PM10.

## 配置
Example config.json

```json
"accessories": [
    {
          "accessory": "Air",
          "apikey": "YOUR_API_KEY",
          "latitude": "YOUR_LATITUDE",
          "longitude": "YOUR_LONGITUDE",
          "name": "Airly Air Quality"
    }
]
```

## 配置文件
字段:
- `accessory` must be "Air" (required).
- `apikey` API key from Airly Developers (required).
- `latitude` String with your latitude e.g. `"52.229676"` (required).
- `longitude` String with your longitude e.g. `"21.012229"` (required).
- `name` Is the name of accessory (required).


## 卸载
> npm install -g homebridge-airly
