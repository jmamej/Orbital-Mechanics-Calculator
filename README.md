# This is a windows forms delta V and orbital velocity calculator

![Orbital mechanics calculator 10 03 2022 13_30_47](https://user-images.githubusercontent.com/57408600/160673920-4c2825aa-8aca-42e5-b1a6-38536d08412d.png)
![Orbital mechanics calculator 10 03 2022 13_33_03](https://user-images.githubusercontent.com/57408600/160673905-933a3681-bcba-410d-8962-ec7c73d0cfdf.png)
![Orbital mechanics calculator 10 03 2022 13_32_48](https://user-images.githubusercontent.com/57408600/160673915-7fb88e6d-48bb-4dec-85ac-c9e41b3ea8e9.png)

## Cheat sheet
- Peryapse - point in orbit closest to the center of mass of primary body.
- Apoapse - point in orbit most distanced from the center of mass of primary body.
- Calculation radius - point in orbit where you want to make a calculation of orbital velocity. Can't be lower than peryapse, can't be higher than apoapse.
- Final radius - in delta v calculation is new peryapse or apoapse after injection.
- Injection into circular orbit - delta v required to turn elliptical orbit into circular.

## Modes
- Orbital velocity
- Delta V

## Selecting primary body
User can chose celestial body being orbited in calculations.

Currently app supports:
- Earth
- Moon
- Sun

## Input variables
- Peryapse
- Apoapse
- Final orbit (for delta V only)
- Calculation orbit (for orbital velocity only)

Calculating even if orbit is below 0. Not a bug it's a feature.

Calculating below negative primary body radius (eg. for Earth below -6371 km) will summon deamons.


# Creating .exe

In cmd install pyinstall:

```
pip pyinstall
```

in cmd with directory of .py file type: 

```
pyinstaller --onefile -w Orbital_Mechanics_Calculator.py
```

# Creating installer

Downlowa NSIS 1.0

.zip directory with .py file

![image](https://github.com/jmamej/Orbital-Mechanics-Calculator/assets/57408600/4fa6d14f-14d1-460c-9e68-132e9a28c5e5)

Installer based on .ZIP file





