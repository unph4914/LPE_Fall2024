# Verification Plan

| **Verification Item**                                          | **Definition of Passing**                                                                                   | **Date Test Performed** | **Test Performed By** | **Measured Result** | **Pass (Y/N)** |
|----------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|--------------------------|------------------------|---------------------|----------------|
| **1. Verify Each Power Supply Voltage (Min & Max)**            | Each power rail remains within ±5% of its specified value.                                                  |                          |                        |                     |                |
| **2. Verify Signal Quality for Each Communication Bus (I2C, UART, SPI)** | Signal levels meet expected thresholds and exhibit low noise. Scope screenshots show clear transitions.     |                          |                        |                     |                |
| **3. Verify Energy Storage Element Charging**                  | Battery charges to its nominal voltage within the specified time at the standard charging current.           |                          |                        |                     |                |
| **4. Verify Power Good Signal and System Boot from Low to Sufficient Charge** | System receives Power Good signal and boots up once energy storage element reaches sufficient charge level. |                          |                        |                     |                |
| **5. Verify System Shutdown as Energy Storage Element Discharges Below Threshold** | System gracefully shuts down once battery voltage reaches cut-off (3.0V).                                  |                          |                        |                     |                |
| **6. Verify Sensors Providing Correct Values to MCU/SoC**       | Sensors (Joystick, Gyro, Ambient Light) provide accurate readings per datasheet specifications.             |                          |                        |                     |                |
| **7. Verify Radio Transmission to Host Device**                | Radio transmits data packets successfully and with no data loss or latency issues.                          |                          |                        |                     |                |
| **8. Verify Radio Reception from Host Device**                 | Radio receives data packets from host device accurately and within latency tolerance.                       |                          |                        |                     |                |
| **9. Verify Energy Harvesting Charges Energy Storage Element** | Solar energy harvesting circuit charges the battery as expected under standard lighting conditions.         |                          |                        |                     |                |
| **10. Verify Target Energy Storage with Energy Harvesting**    | Battery charges to the target level for typical use case (to be confirmed by measurement/calculation).      |                          |                        |                     |                |
| **11. Verify Energy Storage Supports System Without External Charging** | Battery alone powers the system for 7 hours, maintaining all necessary functions (based on 700mAh estimate). |                          |                        |                     |                |
| **12. Verify Each IC (Digital, Analog, Power) is Functional**  | Each IC performs as expected, without fault or overheating.                                                 |                          |                        |                     |                |
| **13. Verify Bulk Capacitance Maintains Voltage**              | Bulk capacitor maintains voltage within design specifications during load fluctuations.                     |                          |                        |                     |                |
| **14. Verify Communication Drivers in Firmware (I2C, SPI, UART)** | All communication protocols transmit and receive data correctly with minimal error rate.                    |                          |                        |                     |                |
| **15. Verify Power Rails Meet Design Voltage Specification**   | Measured voltages of all power rails match design specifications (scope screenshots included in report).    |                          |                        |                     |                |

---

### Additional Notes for Verification

- **Scope Screenshots**: For each power rail, communication bus, and major signal, capture scope screenshots for inclusion in the final report to document measured voltages, currents, and signal quality.
- **Test Equipment**: Plan to use an oscilloscope, multimeter, and power supply for precise measurements during verification.
- **Testing Responsibilities**: Designate team members for each testing task to ensure accountability and streamlined completion.
- **Documentation**: Capture detailed notes, screenshots, and test configurations for any items that do not pass initially, along with corrective actions taken.