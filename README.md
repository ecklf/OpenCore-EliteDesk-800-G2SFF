# HP EliteDesk 800 G2 SFF (Skylake) - macOS 11

OpenCore configuration for macOS Big Sur.

**For educational purposes**. I don't take any responsibility for you voilating the Apple ToS and/or damaging your device.

## Specs

CPU: i5 6500
GPU: HD530
RAM: 8GB
Audio Codec: ALC221
Model: HP EliteDesk 800 G2 SFF
Mobo: Unknown / HP
Ethernet: Intel I219LM

## BIOS

- **Enable** - VTd
- **Enable** - UEFI Boot Order
- **Enable** - Allow PCIe/PCI SERR# Interrupt
- **Disable** - VTx
- **Disable** - Everything in Security (TPM, SureStart etc.)
- **Disable** - SIntel Software Guard Extensions (SGX)
- **Set** - Video memory size **512MB**
- **Set** - Legacy Support Enable and Secure Boot Disable

## Notes

All 10 USB slots are usable, had to map four of the 3.0 to 2.0 for USB power-management though.

Front:
| | | | | | |
| -----|:----:|:----:| :--: | :-------: | :-----------: |
| USB2 | USB2 | USB3 | USB3 | COMBOJACK | HEADPHONEJACK |

Back:
| | |
| :--: |:----:|
| USB2 | LAN |
| USB2 | USB3 |
| USB2 | USB3 |
| USB2 | |

## Not working / WIP

- Sleep
- VGA
- Front Audio I/O
- Dual Monitor (only outer port working atm)
