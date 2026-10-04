## 2. Serial protocol

- **Depends on:** 1
- **Contract:**
  - In: ASCII lines
  - Requires: `PING`→`PONG`; `FLASH <ms>`→`OK <micros>`; error→`ERR <reason>`; parser without hardware
  - Delivers: pure `protocol` module (C++) + protocol docs in the README
- **Pre-work:** none
- **Out of scope:** —
- **Tests:** parser on the native env
