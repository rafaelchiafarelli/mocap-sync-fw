## 3. LED pulse

- **Depends on:** 2
- **Contract:**
  - In: FLASH command
  - Requires: configurable GPIO; duration 20–200 ms; non-blocking
  - Delivers: pulse on the configured pin
- **Pre-work:** Rafael defines the pin, LED and MOSFET (simple schematic)
- **Out of scope:** —
- **Tests:** timing logic on native; manual bench test
