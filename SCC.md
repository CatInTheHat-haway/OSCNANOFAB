# Process for creation of Reflective Lyot Stop 

## Silicon nitride  
Depostion -> [P5000](https://catinthehat-haway.github.io/OSCNANOFAB/P5000)

Deposition Recipe -> "NEW SN"

**average deposition rate**: 335 nm/min

    1 micron layer = 2.985 min = 179.1 sec

Clean Recipe -> "SIN CLEAN"

**Repeat for back side**

## Patterning

1) positive photo resist -> [Spin Coater](https://catinthehat-haway.github.io/OSCNANOFAB/Spin_Coater)

2) prebake: 110C 60s  (hot plate)

3) Pattern -> [MLA150](https://catinthehat-haway.github.io/OSCNANOFAB/MLA150) -> Dose: 200 mJ/cm^2
   
4) postbake: 110C 60s   (hot plate)

5) Develop: MF319 / MF321

6) Plasma etch

**Repeat for back side**

7) KOH wetch etch

## Reflectivity 

Aluminum Deposit -> [Temescal](https://catinthehat-haway.github.io/OSCNANOFAB/Temescal) 
