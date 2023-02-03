# Magic Desk 2
Open Hardware Project to build a 3 in 1 cartridge based on Magic Desk 1MB and Universal c64 Cartridge by Marko Šolajić

3 Different Configuratios
-------------------------
- **Magic Desk 16Kbyte config**
- **Double Magic Desk 1MB**
- **GMod3 2MB Read Only cartridge**

Magic Desk 16Kbyte config
-------------------------
Old Magic Desk Cartridge coul be:
- standard [32Kb (4 banks), 64Kb (8 banks) and 128Kb (16 banks)]
- DDI Magic Cart [32 banks, 256kb]
- Magic Desk Clone homebrew cart [64 banks, 512kb and 128banks, 1MB]

Furthermore:
- ROM is always mapped in at $8000-$9FFF (8k game)
- 1 register at io1 / de00
   - bit 0-6   bank number
   - bit 7     exrom (1 = cart disabled)

**Magic Desk 16Kbyte config**
- supports all "Magic Desk Clone" homebrew cart with 16k game config, up to 2 MB
- ROM is always mapped in at $8000-$BFFF (16k game)
- 1 register at io1 / de00
   - bit 0-6   bank number
   - bit 7     exrom (1 = cart disabled)
So, 128 banks and one bank is 16Kbyte: 2MByte of ROM space.

![PCB](./images/MD2.png)
