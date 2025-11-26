**bbl**key™ security design
===========================

## Overview

The **bbl**key is a transport adapter device that is designed to convert between the KFDtool software protocol and the TIA-102.AACD-A KFD protocol.

| OSI model | KFDtool protocol          | TIA-102.AACD-A KFD protocol | Notes |
|-----------|---------------------------|-----------------------------|-------|
| Layer 1   | USB/UART serial           | Three Wire Interface (TWI)  |
| Layer 1.5 | Command framing           | —                           |
| *Layer 2* | *Exchange session*        | *Exchange session*          | *Passed transparently*
| *Layer 3* | *Key Management Messages* | *Key Management Messages*   | *Passed transparently*

It is **not** a cryptographic device: it does not generate keys, store keys, encrypt or decrypt data, or perform any other function of a cryptographic device.

## Details

| Component                  | Notes |
|----------------------------|-------|
| **Algorithms**             | The **bbl**key does not implement or use any encryption algorithms in hardware or firmware.
| **Cryptographic boundary** | The **bbl**key does not have a cryptographic boundary, as it does not perform any cryptographic operations.
| **Development**            | The **bbl**key is designed and tested in the United States by US nationals.
| **FIPS validation**        | The **bbl**key is not FIPS validated.
| **Firmware security**      | The **bbl**key does not include any firmware secure boot features.
| **Keys**                   | The **bbl**key does not contain any CSPs or keys.
| **Logging**                | The **bbl**key does not perform any logging.
| **Other attacks**          | The **bbl**key is not designed to mitigate any specific attacks outside of those listed in this table, including but not limited to power consumption, timing, fault induction, or TEMPEST attacks.
| **Physical security**      | The **bbl**key does not include any physical anti-tamper features. All components are general-purpose commodity components; no custom components are used.
| **Ports**                  | The **bbl**key provides two physical ports, both of which are used for data input/output. USB-C is additionally used for power and KFDtool software protocol control input and status output. TWI is used for TIA-102.AACD-A KFD protocol.
| **RNG**                    | The **bbl**key does not implement or use any random number generators in hardware or firmware.
| **Roles**                  | The **bbl**key supports one role: user.
| **Software**               | The **bbl**key is compatible with [KFDtool](https://github.com/omahacommsys/KFDtool/) software; please refer to that repository for software security considerations.
| **Storage: non-volatile**  | The **bbl**key does not use any non-volatile memory to store any encryption key material being sent. Product parameters including the model, version, and serial number are stored in non-volatile memory; these values cannot be modified with production firmware. The executable firmware is also stored in non-volatile memory.
| **Storage: volatile**      | The **bbl**key uses the volatile RAM onboard the ATmega328p microcontroller to buffer and frame encryption key material being sent. The **bbl**key does not contain any other volatile memory.

## Disclaimer

The above security details apply to a **bbl**key as manufactured, using original hardware and firmware provided by beep boop labs.

Unauthorized physical or electronic access to the **bbl**key, radios being keyloaded, or computer used to run KFDtool software could result in malicious modifications by a third-party.

⚠️ It is the user's responsibility to maintain physical and electronic control of their **bbl**key device, radios and computers they connect it to, and their encryption key material, at all times to prevent tampering.
