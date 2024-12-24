# nordpool automation Finland fix
Fixing the issue of **nordpool** not updating the electricity prices correctly.
> [!IMPORTANT]  
> **This method will only work if your nordpool integrated is named something along the lines of:** ``sensor.nordpool_kwh_fi_eur_3_10_024``
## Prerequisites
- **nordpool** via **HACS**: [Nordpool Install Guide](https://github.com/custom-components/nordpool?tab=readme-ov-file#installation)

## Steps
1. If you are updating from **nordpool** installation `0.0.15` or earlier, then re-install the **nordpool** integration.
2. Reboot your **Home Assistant** to apply the changes
3. Re-add the integration:
    3.1 Go to ``Settings`` -> ``Devices & Services``<br/>
    3.2 Select ``+ Add Integration``<br/>
    3.3 Search for ``nordpool`` and select it<br/>
    3.4 Fill in the values and Submit<br/>
Your nordpool integrations name should now be something like: ``sensor.nordpool_kwh_fi_eur_3_10_0255`` therefore it's updated.

Now if you use addittional addons then respectively modify the: ``sensor.nordpool_kwh_fi_eur_3_10_024`` into ``sensor.nordpool_kwh_fi_eur_3_10_0255`` through the configs.
