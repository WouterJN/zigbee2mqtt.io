---
title: "DIYRuZ DIYRuZ_FreePad control via MQTT"
description: "Integrate your DIYRuZ DIYRuZ_FreePad via Zigbee2MQTT with whatever smart home
 infrastructure you are using without the vendors bridge or gateway."
---

*To contribute to this page, edit the following
[file](https://github.com/Koenkk/zigbee2mqtt.io/blob/master/docs/devices/DIYRuZ_FreePad.md)*

# DIYRuZ DIYRuZ_FreePad

| Model | DIYRuZ_FreePad  |
| Vendor  | DIYRuZ  |
| Description | [DiY 8/12/20 button keypad](http://modkam.ru/?p=1114) |
| Exposes | battery, action, switch_type, switch_actions, linkquality |
| Picture | ![DIYRuZ DIYRuZ_FreePad](../images/devices/DIYRuZ_FreePad.jpg) |

## Notes


### Firmware
Open source firmware can be found here: [Github](https://github.com/diyruz/freepad)

### How to join:
#### If device in FN(factory new) state:
1. Press and hold button (1) for 2-3 seconds, until device start flashing led
2. Wait, in case of successful join, device will flash led 5 times
3. If join failed, device will flash led 3 times

#### If device in a network:
1. Hold button (1) for 10 seconds, this will reset device to FN(factory new) status
2. Go to step 1 for FN device

### How to use touch link
1. Bring you remote near to TL device
2. Hold button (2) for 5 seconds
TL funtionality can work without connecting to network



## Exposes
### Battery (numeric)
Remaining battery in %.
Value can be found in the published state on the `battery` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The minimimal value is `0` and the maximum value is `100`.
The unit of this value is `%`.

### Action (enum)
Triggered action (e.g. a button click).
Value can be found in the published state on the `action` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The possible values are: `*_single`, `*_double`, `*_triple`, `*_quadruple`, `*_release`.

### Switch_type (enum, button_1 endpoint)
Value can be found in the published state on the `switch_type_button_1` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_1": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_1": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_1 endpoint)
Value can be found in the published state on the `switch_actions_button_1` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_1": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_1": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_2 endpoint)
Value can be found in the published state on the `switch_type_button_2` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_2": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_2": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_2 endpoint)
Value can be found in the published state on the `switch_actions_button_2` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_2": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_2": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_3 endpoint)
Value can be found in the published state on the `switch_type_button_3` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_3": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_3": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_3 endpoint)
Value can be found in the published state on the `switch_actions_button_3` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_3": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_3": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_4 endpoint)
Value can be found in the published state on the `switch_type_button_4` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_4": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_4": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_4 endpoint)
Value can be found in the published state on the `switch_actions_button_4` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_4": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_4": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_5 endpoint)
Value can be found in the published state on the `switch_type_button_5` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_5": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_5": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_5 endpoint)
Value can be found in the published state on the `switch_actions_button_5` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_5": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_5": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_6 endpoint)
Value can be found in the published state on the `switch_type_button_6` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_6": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_6": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_6 endpoint)
Value can be found in the published state on the `switch_actions_button_6` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_6": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_6": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_7 endpoint)
Value can be found in the published state on the `switch_type_button_7` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_7": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_7": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_7 endpoint)
Value can be found in the published state on the `switch_actions_button_7` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_7": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_7": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_8 endpoint)
Value can be found in the published state on the `switch_type_button_8` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_8": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_8": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_8 endpoint)
Value can be found in the published state on the `switch_actions_button_8` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_8": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_8": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_9 endpoint)
Value can be found in the published state on the `switch_type_button_9` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_9": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_9": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_9 endpoint)
Value can be found in the published state on the `switch_actions_button_9` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_9": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_9": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_10 endpoint)
Value can be found in the published state on the `switch_type_button_10` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_10": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_10": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_10 endpoint)
Value can be found in the published state on the `switch_actions_button_10` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_10": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_10": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_11 endpoint)
Value can be found in the published state on the `switch_type_button_11` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_11": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_11": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_11 endpoint)
Value can be found in the published state on the `switch_actions_button_11` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_11": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_11": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_12 endpoint)
Value can be found in the published state on the `switch_type_button_12` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_12": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_12": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_12 endpoint)
Value can be found in the published state on the `switch_actions_button_12` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_12": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_12": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_13 endpoint)
Value can be found in the published state on the `switch_type_button_13` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_13": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_13": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_13 endpoint)
Value can be found in the published state on the `switch_actions_button_13` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_13": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_13": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_14 endpoint)
Value can be found in the published state on the `switch_type_button_14` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_14": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_14": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_14 endpoint)
Value can be found in the published state on the `switch_actions_button_14` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_14": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_14": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_15 endpoint)
Value can be found in the published state on the `switch_type_button_15` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_15": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_15": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_15 endpoint)
Value can be found in the published state on the `switch_actions_button_15` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_15": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_15": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_16 endpoint)
Value can be found in the published state on the `switch_type_button_16` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_16": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_16": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_16 endpoint)
Value can be found in the published state on the `switch_actions_button_16` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_16": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_16": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_17 endpoint)
Value can be found in the published state on the `switch_type_button_17` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_17": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_17": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_17 endpoint)
Value can be found in the published state on the `switch_actions_button_17` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_17": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_17": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_18 endpoint)
Value can be found in the published state on the `switch_type_button_18` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_18": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_18": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_18 endpoint)
Value can be found in the published state on the `switch_actions_button_18` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_18": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_18": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_19 endpoint)
Value can be found in the published state on the `switch_type_button_19` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_19": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_19": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_19 endpoint)
Value can be found in the published state on the `switch_actions_button_19` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_19": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_19": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Switch_type (enum, button_20 endpoint)
Value can be found in the published state on the `switch_type_button_20` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_type_button_20": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_type_button_20": NEW_VALUE}`.
The possible values are: `toggle`, `momentary`, `multifunction`.

### Switch_actions (enum, button_20 endpoint)
Value can be found in the published state on the `switch_actions_button_20` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"switch_actions_button_20": ""}`.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"switch_actions_button_20": NEW_VALUE}`.
The possible values are: `on`, `off`, `toggle`.

### Linkquality (numeric)
Link quality (signal strength).
Value can be found in the published state on the `linkquality` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The minimimal value is `0` and the maximum value is `255`.
The unit of this value is `lqi`.

## Manual Home Assistant configuration
Although Home Assistant integration through [MQTT discovery](../integration/home_assistant) is preferred,
manual integration is possible with the following configuration:


{% raw %}
```yaml
sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    unit_of_measurement: "%"
    value_template: "{{ value_json.battery }}"
    device_class: "battery"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.action }}"
    icon: "mdi:gesture-double-tap"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_1 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_1 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_2 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_2 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_3 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_3 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_4 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_4 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_5 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_5 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_6 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_6 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_7 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_7 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_8 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_8 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_9 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_9 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_10 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_10 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_11 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_11 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_12 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_12 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_13 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_13 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_14 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_14 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_15 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_15 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_16 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_16 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_17 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_17 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_18 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_18 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_19 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_19 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_type_button_20 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    value_template: "{{ value_json.switch_actions_button_20 }}"

sensor:
  - platform: "mqtt"
    state_topic: "zigbee2mqtt/<FRIENDLY_NAME>"
    availability_topic: "zigbee2mqtt/bridge/state"
    unit_of_measurement: "lqi"
    value_template: "{{ value_json.linkquality }}"
    icon: "mdi:signal"
```
{% endraw %}


