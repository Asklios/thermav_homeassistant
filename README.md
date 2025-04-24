# LG Therma V - Home Assistant
Home Assistant Modbus config for the LG Therma V Heatpump

## Installation
1. Copy the YAML file (`modbus_hp.yaml`) to your Home Assistant `configuration/integrations` directory
2. Add the following to your `secrets.yaml`:
   ```yaml
   lg_heatpump_modbus_host_ip: YOUR_IP_ADDRESS
   lg_heatpump_modbus_port: YOUR_PORT
   lg_heatpump_modbus_slave: YOUR_SLAVE_ID
   ```
3. Include the configuration files in your `configuration.yaml`
   ```yaml
   homeassistant:
     packages: !include_dir_named integrations
   ```
4. Restart Home Assistant

## Requirements
- Home Assistant (confirmed working with 2025.2.2)
- LG Therma V heat pump with Modbus connectivity

## Acknowledgments
Automations inspired by [basti242/homeassistant_lg_therma_v_modbus](https://github.com/basti242/homeassistant_lg_therma_v_modbus/tree/main). Check their [wiki](https://github.com/basti242/homeassistant_lg_therma_v_modbus/wiki) for additional usage information.
