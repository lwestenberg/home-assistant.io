---
title: Bold
description: Instructions on how to integrate Bold within Home Assistant.
ha_category:
  - Lock
ha_release: 2022.12
ha_iot_class: Cloud Polling
ha_config_flow: true
ha_codeowners:
  - '@lwestenberg'
ha_domain: bold
ha_platforms:
  - lock
ha_integration_type: integration
---

The Bold integration controls your Bold Smart Lock using the official [Bold](https://boldsmartlock.com/) API. There is currently support for the following device types within Home Assistant:

- [Lock](#lock)

<div class="note warning">

You need a Bold Connect to use this integration as it is used by the API to remotely unlock the smart lock. We are working on an update in which Home Assistant can serve as the Controller via Bluetooth.

</div>

{% include integrations/config_flow.md %}

### Lock

The lock platform allows you to unlock a Bold Smart Lock. A lock entity will be added for each Bold Smart Lock that is configured in your account.
