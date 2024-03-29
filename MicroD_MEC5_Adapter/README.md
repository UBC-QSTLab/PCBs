# Micro-D to MEC5 Adapter PCB

This PCB is designed to allow us to use the DC sample holder from the fridge in Josh Folk's dipstick by converting the Micro-D connector to a MEC5 (card edge) connection.

![](img/Layout_Both.png)

## General Notes

* The numbers near the card edge are the card edge pin numbering which is NOT the same as the breakout box pin numbering
    * However the board is routed so the sample (or Micro-D) pin numbers match the breakout box
* The partially exposed copper "ground" plane is connected to pins 1, 3, 5, 7, 9, 51, 53, 55, 57, 59 of the card edge connector which should be grounded
* The pins of the Micro-D connector should be cut to be flush with the bottom of the PCB, soldered, and then wrapped in Teflon tape so they don't get shorted by the metal block in the dipstick

## Ordering Information

| Parameter                           | Value                        | Notes |
| ----------------------------------- | ---------------------------- | ----- |
| Gold fingers                        | Yes                          | |
| Gold finger surface finish          | Hard Gold (Au:10U"/Ni:120U") | Hard Gold allows for more insertion cycles into a card edge connector |
| Gold finger bevel edge              | 30 deg                       | Bevel makes insertion easier, this is a pretty standard value |
| Gold finger bevel hypotenuse length | 0.9 mm                       | This value was recommended by PCBgogo |
| Pad surface finish                  | ENIG                         | |

## BOM

| Part Number | Manufacturer | Description | Notes |
| ----------- | ------------ | ----------- | ----- |
| [581-M25-213L461](https://www.digikey.ca/en/products/detail/norcomp-inc/581-M25-213L461/13557502) | NorComp Inc. | Female (Receptacle) Micro-D Connector | |

## Pin Mapping (Summary)

All the pin numbers stay the same except for 13 and 16 which map to 33 and 36 respectively.

| Micro-D Pin  | Dipstick Breakout Board Pin |
| ------------ | --------------------------- |
| 1            | 1                           |
| 2            | 2                           |
| 3            | 3                           |
| 4            | 4                           |
| 5            | 5                           |
| 6            | 6                           |
| 7            | 7                           |
| 8            | 8                           |
| 9            | 9                           |
| 10           | 10                          |
| 11           | 11                          |
| 12           | 12                          |
| <font color="red">13</font> | <font color="red">33</font> |
| 14           | 14                          |
| 15           | 15                          |
| <font color="red">16</font> | <font color="red">36</font> |
| 17           | 17                          |
| 18           | 18                          |
| 19           | 19                          |
| 20           | 20                          |
| 21           | 21                          |
| 22           | 22                          |
| 23           | 23                          |
| 24           | 24                          |
| 25           | 25                          |

### Micro-D Pin Numbering

![](img/Adapter_MicroD_Pinout.png)

## Pin Mapping (Full Detail)

| Micro-D Pin  | Dipstick Breakout Board Pin | MEC5 (Card Edge) Pin |
| ------------ | --------------------------- | -------------------- |
| 1            | 1                           | 60                   |
| 2            | 2                           | 58                   |
| 3            | 3                           | 56                   |
| 4            | 4                           | 54                   |
| 5            | 5                           | 52                   |
| 6            | 6                           | 50                   |
| 7            | 7                           | 49                   |
| 8            | 8                           | 48                   |
| 9            | 9                           | 47                   |
| 10           | 10                          | 46                   |
| 11           | 11                          | 45                   |
| 12           | 12                          | 44                   |
| 13           | 33                          | 23                   |
| 14           | 14                          | 42                   |
| 15           | 15                          | 41                   |
| 16           | 36                          | 20                   |
| 17           | 17                          | 39                   |
| 18           | 18                          | 38                   |
| 19           | 19                          | 37                   |
| 20           | 20                          | 36                   |
| 21           | 21                          | 35                   |
| 22           | 22                          | 34                   |
| 23           | 23                          | 33                   |
| 24           | 24                          | 32                   |
| 25           | 25                          | 31                   |
| NC           | 26                          | 30                   |
| NC           | 27                          | 29                   |
| NC           | 28                          | 28                   |
| NC           | 29                          | 27                   |
| NC           | 30                          | 26                   |
| NC           | 31                          | 25                   |
| NC           | 32                          | 24                   |
| NC           | 34                          | 22                   |
| NC           | 35                          | 21                   |
| NC           | 37                          | 19                   |
| NC           | 38                          | 18                   |
| NC           | 39                          | 17                   |
| NC           | 40                          | 16                   |
| NC           | 41                          | 15                   |
| NC           | 42                          | 14                   |
| NC           | 43                          | 13                   |
| NC           | 44                          | 12                   |
| NC           | 45                          | 11                   |
| NC           | 46                          | 10                   |
| NC           | 47                          | 8                    |
| NC           | 48                          | 6                    |
| NC           | 49                          | 4                    |
| NC           | 50                          | 2                    |
| NC           | GND                         | 1, 3, 5, 7, 9, 51, 53, 55, 57, 59 |

### MEC5 (Card Edge) Pin Numbering

![](img/Layout_Top.png) ![](img/Layout_Bottom.png)