**bbl**key™
============

The **bbl**key is a P25 keyloader that allows the keyloading of TIA-102 standards-compliant radios when used with [KFDtool](https://github.com/omahacommsys/KFDtool/) software.

## The **bbl**key advantage

Unlike competing devices such as the KFDmicro and KFDpico, the **bbl**key is designed from the start for a premium experience:

- Genuine FTDI UART chip (no driver issues)
- Durable aluminum enclosure
- Recessed USB-C connector with quality USB-A to USB-C cable included
- Exclusive improved [Rust](https://rust-lang.org/) firmware
- Top-tier after-sale support from [KFDtool](https://github.com/omahacommsys/KFDtool/) developers

## 🛒 [Order now!](https://shop.beepbooplabs.ltd/products/bblkey)

![**bbl**key with included USB and hirose cables](images/bblkey.jpg)

## Compatibility

The **bbl**key is guaranteed to work with the following tested radios, keyloaders, and software.

*Have you used a **bbl**key with a different radio or software? [Please let us know!](mailto:contact@beepbooplabs.ltd)*

### Radios

The following radios have been tested for compatibility at this time:

| Radio series                  | Support status | Notes |
|-------------------------------|----------------|-------|
| Aeroflex IFR 2975             | ✅ Tested      |
| Bendix-King BKR               | ✅ Tested      |
| Bendix-King KNG               | ✅ Tested      |
| EF Johnson VP/VM x000         | ✅ Tested      |
| EF Johnson VP/VM x00          | ✅ Tested      |
| EF Johnson 5100/ES            | ✅ Tested      |
| Harris XG-100P                | ✅ Tested      |
| Harris XG-100M (via CH100)    | ✅ Tested      |
| Harris XG mobile (via 44-pin) | ✅ Tested      | Requires 14002-0143-10 adapter
| Harris XG portable            | ❔ Untested    | Requires 14002-0143-01 adapter
| Harris XL mobile              | ✅ Tested      | Requires [**XL**key™](https://github.com/beepbooplabsltd/xlkey) or 14050-6350-01 or -02 adapter
| Harris XL portable            | ✅ Tested      |
| Kenwood NX                    | ✅ Tested      | Requires SCM module
| Kenwood TK                    | ❔ Untested    | Requires SCM module
| Motorola APX                  | ✅ Tested      |
| Motorola ASTRO25 (MACE)       | ✅ Tested      | Requires MACE module
| Motorola ASTRO25 (UCM)        | ✅ Tested      | Requires UCM module
| Motorola ASTRO                | ✅ Tested      | Requires EMC module
| Motorola R2670                | ✅ Tested      |
| Tait TP/TM 9x00               | ✅ Tested      | Requires [kiwi**key**™](https://github.com/beepbooplabsltd/kiwikey) or TPA-SV-020 adapter
| Thales Liberty                | ✅ Tested      |

### Keyloaders

The following keyloaders have been tested for compatibility (sharing keys) at this time:

| Keyloader              | From **bbl**key  | To **bbl**key | Notes |
|------------------------|------------------|---------------|-------|
| Motorola KVL 3000      | ❌ Not supported | ✅ Tested     |
| Motorola KVL 3000+     | ❌ Not supported | ✅ Tested     |
| Motorola KVL 4000      | ✅ Tested        | ✅ Tested     |
| Motorola KVL 5000      | ✅ Tested        | ✅ Tested     |
| Motorola KVL 7000      | ❔ Untested      | ❔ Untested   |
| Tait EnableProtect KFD | ❔ Untested      | ❔ Untested   | Requires T03-00059-AAAA KFD to TIA adapter

### Software

The **bbl**key is designed to work with the OCS fork of the open-source [KFDtool](https://github.com/omahacommsys/KFDtool/) software, version [**1.8.8**](https://github.com/omahacommsys/KFDtool/releases/tag/1.8.8), and we will continue to support this release despite the project being archived.

While not officially supported, the **bbl**key should work with software designed for the KFDshield protocol, including mobile apps and the [KFDweb](https://github.com/grover556/KFDweb) browser-based tool.

We are carefully monitoring the future of the keyloading software ecosystem and continually evaluating compatibility and potential improvements.

## Firmware

### Firmware versions

**bbl**keys ship with the latest firmware available at time of order:

| Firmware release | Version | Orders on or after | Release notes |
|------------------|---------|--------------------|---------------|
| `bblkey_A1`      | 2.0.1   | Launch             | Reduces false failure indications during adapter self-test
| `bblkey_A0`      | 2.0.0   | Pre-release        | —

### Firmware updates

The **bbl**key is designed easily be updated at home if a user wishes.

Instructions will be provided when the first notable firmware update is released.

## Security design

As with any device that may come in contact with encryption key material, it is important to understand the security design and risk factors when using the **bbl**key.

For more information, please review the in-depth discussion of the [**bbl**key security design](./security-design.md).

## Legal

The names "beep boop labs" and "**bbl**key", and the alembic distiller and keyhole logos, are trademarks and/or copyrighted works of beep boop labs ltd. All rights are reserved.

Any reference to KFDtool, KFDmicro, Motorola, or any other third party manufacturer, or any of their products, is for informational purposes only. No representation is made that any such manufacturer has endorsed beep boop labs ltd or its products.
