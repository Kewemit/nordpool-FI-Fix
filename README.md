# Home Assistant Nordpool fix
I believe due to the VAT changing from ``24%`` to ``25.5%`` in Finland, the nordpool plugin broke.

This will cover the issue of **nordpool** not updating the electricity prices correctly.
> [!IMPORTANT]  
> **This method will work if your nordpool integrated is named something along the lines of:** ``sensor.nordpool_kwh_fi_eur_3_10_024``
## Prerequisites
- **nordpool** via **HACS**: [Nordpool Install Guide](https://github.com/custom-components/nordpool?tab=readme-ov-file#installation)
## Steps
1. If you are updating from **nordpool** `0.0.15` or earlier, then **re-install** the nordpool integration. (**<ins>re-installing is very important!</ins>**)
2. Reboot your **Home Assistant** to apply the changes
3. Re-add the integration via: <br/>
    3.1 ``Settings`` -> ``Devices & Services``<br/>
    3.2 Select ``+ Add Integration``<br/>
    3.3 Search for ``nordpool`` and select it<br/>
    3.4 Fill in the values and Submit<br/>
    
Your nordpool integration's name should now be something like: ``sensor.nordpool_kwh_fi_eur_3_10_0255`` therefore it's updated. Now if you use additional addons then modify the: ``sensor.nordpool_kwh_fi_eur_3_10_024`` into ``sensor.nordpool_kwh_fi_eur_3_10_0255`` through their respective configs.
