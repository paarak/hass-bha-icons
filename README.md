# hass-bha-icons

Custom icon pack designed for Home Assistant.

## Content

![Preview](./svg/ceiling-lamp.svg) ceiling-lamp<br />
![Preview](./svg/ceiling-lamp-plafond.svg) ceiling-lamp-plafond<br />
![Preview](./svg/ceiling-lamp-round.svg) ceiling-lamp-round<br />
![Preview](./svg/chandelier.svg) chandelier<br />
![Preview](./svg/floor-lamp.svg) floor-lamp<br />
![Preview](./svg/floor-lamp-dual.svg) floor-lamp-dual<br />
![Preview](./svg/led-strip.svg) led-strip<br />
![Preview](./svg/light-string.svg) light-string<br />
![Preview](./svg/outdoor-lamp.svg) outdoor-lamp<br />
![Preview](./svg/outdoor-lamp-solo.svg) outdoor-lamp-solo<br />
![Preview](./svg/outdoor-lamp-variant.svg) outdoor-lamp-variant<br />
![Preview](./svg/mirror-lamp.svg) mirror-lamp<br />
![Preview](./svg/roborock.svg) roborock<br />
![Preview](./svg/smoke-detector.svg) smoke-detector<br />
![Preview](./svg/thermostat.svg) thermostat<br />
![Preview](./svg/xmas-candle-bridge.svg) xmas-candle-bridge<br />
![Preview](./svg/xmas-star.svg) xmas-star<br />


## Install

Copy the `hass-bha-icons.js` file into `<config>/www/` where `<config>` is your home-assistant config directory (the directory where your `configuration.yaml` resides).

Add the folowing to the `frontend` section of your `configuration.yaml`

```yaml
frontend:
  extra_module_url:
    - /local/hass-bha-icons.js
```

Restart home-assistant.

## Using

The icons uses the prefix `bha:`.

Example:

```
entities:
  - entity: light.floor_lamp
    icon: 'bha:floor-lamp'
    name: floor-lamp
  - entity: light.floor_lamp_dual
    icon: 'bha:floor-lamp-dual'
    name: floor-lamp-dual
  - entity: light.led_strip
    icon: 'bha:led-strip'
    name: led-strip
  - entity: light.outdoor_lamp_north
    icon: 'bha:outdoor-lamp'
    name: outdoor-lamp
  - entity: light.outdoor_lamp_west
    icon: 'bha:outdoor-lamp-variant'
    name: outdoor-lamp-variant
show_header_toggle: false
title: hass-bha-icons
type: entities
```

## FAQ

Q: The icon ain't showing, it's just white space where it should be. What's up with that?

A: Probably related to cache. Try opening your instance in a incognito/private Window and see if your icon shows then. If yes, it's cache related. If not, spellcheck.

## Thanks

Thanks to @thomasloven, as I used his hass-fontawesome as a template for this pack 
