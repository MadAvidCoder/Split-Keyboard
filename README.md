# Split Keyboard
An ergonomic, wireless, split, low-profile keyboard I made for [Hack Club](https://hackclub.com/) [Blueprint](https://blueprint.hackclub.com/r/43?ref=r)! It is inspired by the Lily58 layout, but with column-staggering better optimised for my hands. It also features a thumb cluster designed for better ergonomics. Having recently started using a Mechcanical Keyboard, I was keen to design a Split Keyboard that was easy to transition to, so I elected to include a number row, and an additional 'function' column on each half.

You can read about my development journey [here](https://blueprint.hackclub.com/projects/10297).

<img width="747" height="420" alt="render" src="https://github.com/user-attachments/assets/c8ddad2c-a0f7-4b73-a12a-eafe7b765c28" />

## Key Features
- Wireless
- Split
- Customisable ZMK Firmware
- Column Staggered
- 54 Keys
- Thumb Clusters
- Low Profile Choc Switches
- RGB Backlight

## PCB
I designed the PCB using KiCad. I kept it simple, with only 2 layers. The two halves are (mostly) mirror-images of each other, and I used hierarchical sheets to easily keep the design matching.

### Schematic
<img width="2200" height="1700" alt="schematic" src="https://github.com/user-attachments/assets/34ca9530-407e-4485-b407-1ef528ce07ca" />

### PCB Design
| Left | Right |
|------|------|
|<img alt="image" src="https://github.com/user-attachments/assets/ef542dc7-7ea3-49c0-95cd-e7d6cbaa7627" />|<img alt="image" src="https://github.com/user-attachments/assets/2ac5e8eb-bead-4c70-936a-61b88e39289c" />|

## Firmware
I am using [ZMK Firmware](https://zmk.dev/) for this keyboard. The configuration files are in their own repo, linked to the `firmware` directory. I chose to keep the keymap simple, to make it easy to transition to from a standard keyboard. I have also included minimal extra features and config, as I want to experiment with that side of things, once I have actually built it.

## Case
I designed the case for the keyboard in Autodesk Fusion 360. It is a fairly simple design, which secures the PCB via 5 screws, and has a top plate to hold it all in place. The top half is secured with a number of locating pins. The two halves of the case are nearly identical, except for different placement of the capacitor cutout.

The case also features a cutout and location for the LiPo battery, so it can be easily secured. USB and charging access is via the edge above the thumb cluster.

|Top|Bottom|
|---|------|
|<img width="685" height="560" alt="image" src="https://github.com/user-attachments/assets/00c2fe81-15e1-4eca-a211-f15b0a7c6a1c" />|<img width="499" height="398" alt="image" src="https://github.com/user-attachments/assets/07f16f96-ab2c-49f4-ab26-3b76283fcd87" />|

### Render
<img width="747" height="420" alt="render" src="https://github.com/user-attachments/assets/c8ddad2c-a0f7-4b73-a12a-eafe7b765c28" />

### Keycaps
To ensure they work well, I am using keycaps designed by other people. For the main keycaps, I am using the [LPX profile keycaps](https://github.com/levpopov/LPX), designed by [levpopov](https://github.com/levpopov).

For the thumb clusters, I have selected the [Choc Louder Keycaps](https://www.printables.com/model/1066117-choc-louder-keycaps-choc-and-mx-spacing) by [kooziecup](https://www.printables.com/@koozie). The dimpled profile should make them more comfortable for the thumbs to rest on.

## BOM
A more detailed csv BOM can be found in [BOM.csv](/BOM.csv). All prices are in USD, and rounded to 2 decimal places (although the total is based on un-rounded prices).

In some cases, items may have higher quantities than are actually needed, due to MOQ. However, I have done thorough research to ensure that these still work out as the cheapest option.

| Item                    | Qty. | Price (USD) | Ext. Price (USD) | Link                                                  |
|-------------------------|------|-------------|------------------|-------------------------------------------------------|
| PCB                     | 1    | 12.55       | 12.55            | https://jlcpcb.com/                                   |
| Battery                 | 2    | 5.80        | 11.60            | https://ecocell.com.au/product/lipo-600-503040/       |
| nice!nano               | 2    | 4.55        | 9.10             | https://www.aliexpress.com/item/1005007266900944.html |
| Hotswap Sockets         | 70   | 0.11        | 7.70             | https://www.aliexpress.com/item/1005009312876316.html |
| Switches                | 60   | 0.46        | 27.60            | https://www.aliexpress.com/item/1005008751312031.html |
| SK6812-MINI-E           | 55   | 0.07        | 3.85             | https://www.lcsc.com/product-detail/C5149201.html     |
| DMBJ PNLS8040-100M 10UH | 5    | 0.11        | 0.55             | https://www.lcsc.com/product-detail/C2849554.html     |
| 100nF Capacitor         | 100  | 0.01        | 1.00             | https://www.lcsc.com/product-detail/C49678.html       |
| 10uF Capacitor          | 10   | 0.02        | 0.20             | https://www.lcsc.com/product-detail/C32635.html       |
| 22uF Capacitor          | 10   | 0.02        | 0.20             | https://www.lcsc.com/product-detail/C98190.html       |
| 470uF Capacitor         | 10   | 0.04        | 0.40             | https://www.lcsc.com/product-detail/C2858856.html     |
| 1N5819 Diode            | 100  | 0.01        | 1.00             | https://www.lcsc.com/product-detail/C963381.html      |
| SS34 Schottky Diode     | 10   | 0.03        | 0.30             | https://www.lcsc.com/product-detail/C842788.html      |
| 806k Resistor           | 20   | <0.01       | 0.09             | https://www.lcsc.com/product-detail/C865659.html      |
| 2M Resistor             | 100  | <0.01       | 0.25             | https://www.lcsc.com/product-detail/C26112.html       |
| 470R Resistor           | 100  | <0.01       | 0.17             | https://www.lcsc.com/product-detail/C2907267.html     |
| 2k Resistor             | 100  | <0.01       | 0.18             | https://www.lcsc.com/product-detail/C2907248.html     |
| 10k Resistor            | 10   | 0.04        | 0.40             | https://www.lcsc.com/product-detail/C319942.html      |
| 73.2k Resistor          | 50   | 0.01        | 0.50             | https://www.lcsc.com/product-detail/C422816.html      |
| 330R Resistor           | 100  | <0.01       | 0.13             | https://www.lcsc.com/product-detail/C2907321.html     |
| DW01A                   | 20   | 0.02        | 0.40             | https://www.lcsc.com/product-detail/C18164398.html    |
| FS8205                  | 10   | 0.05        | 0.50             | https://www.lcsc.com/product-detail/C2830320.html     |
| MT3608                  | 10   | 0.06        | 0.60             | https://www.lcsc.com/product-detail/C84817.html       |
| LCSC Shipping           | 1    | 12.72       | 12.72            | https://www.lcsc.com/                                 |
| EcoCell Shipping        | 1    | 2.78        | 2.78             | https://ecocell.com.au/                               |