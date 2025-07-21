# PLC Logic for Conveyor Belt System

## 👷 Project Scenario

- **Start Button (I1):** Starts the conveyor motor.
- **Reset Button (I2):** Resets the object counter and restarts the system.
- **Sensor (I3 - XUB5BPANL2):** Detects marble blocks on the belt.
- **Conveyor Motor (Q1):** Motor output controlled by logic.
- **Counter (C1):** Stops motor after 5 detections.

---

## 🔁 Ladder Logic Description

### 1. Start and Stop Logic
- When `I1` is pressed, `Q1` is latched (self-holding).
- When `C1` reaches 5, it resets `Q1`.

### 2. Counting Logic
- On each rising edge of `I3`, `C1` increments by 1.
- `C1` preset value = 5.

### 3. Reset Logic
- When `I2` is pressed, `C1` is reset, and `Q1` is re-enabled.

---

## 🧠 Logic Flow

```plaintext
[Start Button (I1)] --| |-------------+--( )--> [Q1 - Conveyor Motor]
                      |               |
                [Q1]--| | (latching)   |
                      |               +--[I3 ↑]--> [C1++]
                      |
       [C1 >= 5] ----|/|-------------| R |--> [Q1 stops]

[Reset Button (I2)] --| |-------------| R |--> [C1 = 0]
