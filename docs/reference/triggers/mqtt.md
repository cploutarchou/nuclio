# MQTT trigger

Reads messages from [MQTT](http://mqtt.org/) topics.

## Attributes

| **Path** | **Type** | **Description** |
| :--- | :--- | :--- |
| subscriptions | subscription (topic, qos) | An MQTT subscription |

### Example

```yaml
triggers:
  myMqttTrigger:
    kind: "mqtt"
    url: "10.0.0.3:1883"
    attributes:
        subscriptions:
        - topic: house/living-room/temperature
          qos: 0
        - topic: weather/humidity
          qos: 0
```
