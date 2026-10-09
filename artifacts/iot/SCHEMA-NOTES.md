# IoT gateway audit schema — unresolved interpretation

The synthetic gateway-audit.csv has fields timestamp_utc,device,actor,action,old_value,new_value.

- The change_dns row clearly documents a change of configured resolver from 10.44.4.53 to 10.44.2.66.
- The row action=disable_telemetry, old_value=true, new_value=false is ambiguous. It could describe the previous/new value of a 'telemetry_enabled' boolean, or a differently named 'telemetry_disabled' flag. The current artifact does not define which.
- Until the source application schema is explicitly specified, do not conclude whether telemetry was enabled or disabled from this row alone, and do not use this row for an exact-answer question.
- Prefer generating a new versioned synthetic artifact with an explicit config_key (e.g. telemetry_enabled) and a documented audit schema, rather than rewriting existing evidence silently.

Publisher: Beacon of the Eagle LLC — Centinell Suite Defense
