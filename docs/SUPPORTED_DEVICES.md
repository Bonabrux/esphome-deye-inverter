# Supported Devices

## 📋 Currently Supported Inverters

- **Deye SG0XLP1** *(Single Phase Low Voltage)*
   
  ***Single Phase Recommended baud rate: 9600 (default, nothing to change)***

  Firmware 3389-1515 and newer (Modbus protocol V118): use `pv_inverter/deye_hybrid_1p_lv_v118.yaml` instead of `pv_inverter/deye_hybrid_1p_lv.yaml`. It adds per-weekday Time of Use, Time of Use slot modes (Grid/Gen charge, GM, BU, CH), CT/meter configuration (register 326), external meter readings and full alarm/fault decoding. Older firmwares keep using `deye_hybrid_1p_lv.yaml`.

- **Deye SG04LP3** *(Low Voltage)*
- **Deye SG05LP3** *(Low Voltage)*
- **Deye SG01HP3** *(High Voltage)*
- **Deye SG02HP3** *(High Voltage)*
   
  ***3 Phases Recommended baud rate: 9600 (default, nothing to change)***

### Deye Inverter Configuration

To set the baud rate on your Deye inverter:
1. Navigate to: **Advanced Settings** → **Paral. Set 3** → **Boud Rate**
2. Set the value to **9600**
3. Save the settings


**Note**: After saving, the screen will turn off and a red LED alarm will flash - this is normal behavior. Everything should return to normal after a moment.
