## 📄 calibration-procedures.md

### Mercury Flow Calibration

1. Initialize sensor interface (`sensor_interface.py`)
2. Power on mercury heater loop (if applicable)
3. Use Doppler flow sensor to read flow velocity
4. Adjust tilt, rotation, or convection to achieve ~0.5 m/s
5. Record and confirm steady state for 2 minutes

### Sensor Health Check

- Thermal sensors: should return 20–250°C range
- Capacitive/resistive sensors: zero-drift check
- Pressure sensor: verify against reference vacuum

### AI Boot Test

- Confirm Jetson/Nvidia controller boots within 10s
- Validate GPIO pins and I2C bus for sensor interface
- Begin logging from `mhd_monitor.py`

---
