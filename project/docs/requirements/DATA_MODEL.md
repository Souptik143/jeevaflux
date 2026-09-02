# Data Model

## User

```text
user_id
baseline_profile
context_preferences
consent_settings
created_at
updated_at
```

## SensorReading

```text
reading_id
timestamp
device_id
sensor_type
value
unit
quality_flag
```

## EnvironmentalReading

```text
reading_id
timestamp
temperature
humidity
pm25
pm10
air_quality_indicator
quality_flag
```

## RiskEvent

```text
event_id
timestamp
risk_type
severity
confidence
contributing_features
alert_status
acknowledged_at
```

## DeviceState

```text
device_id
battery_level
connectivity_state
firmware_version
model_version
sensor_status
timestamp
```

## SyncRecord

```text
record_id
authorization_state
sync_state
last_attempt
last_success
```

## Data Minimization

Only fields required for the enabled functionality should be retained or
synchronized.
