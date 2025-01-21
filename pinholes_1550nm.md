# Multi‐pinhole mask fabrication for 1550 nm light

[MLA/SEM Images](https://github.com/CatInTheHat-haway/OSCNANOFAB/blob/main/pinhole_sem.pdf)

## Preparation of sample

**Prep Sample Slides**
* Cut microscope slide into 3 pieces
* Clean slides with acetone and dry with nitrogen air

**oxygen plasma bake in microwave**
* Put in sample, cover with glass dish
* White Switch —> vacuum on
* System vacuum —> on
* Gas Control —> on
* Time —> 5 minutes 
* Gas control —>off
* System Vaccuum —> off
* White switch —> vacuum off
* Take out sample 

## Adhesion + Photoresist 

**Use syringe to put HDMS (adhesion) on sample**
* Solvent 
* Use under fume hood on hotplate 
* Put HDMS on blank slides (not the sample slides) using syringe 
* Syringe goes in sharps
* Temp —> 18C / 60C ?
* Lid on + Time —> 5 mins
* Take out sample —> hot plate and light off, close fume hood door

**Add photo resist with spin coater machine**
* Clean photoresist bottle with acetone
* Wipe is dry waste
* Want photo resist to be room temp, but need to store in fridge
* Turn machine on with black button on the back
* Place sample on vacuum (+ turn on vacuum)
* Add photo resist (chemical?) with syringe + 2mm (?) filter 
* Spin with machine
* Run mode —> static program process  
* Line machine with foil and clean up immediately. Use syringe with needle to get chemicals out of bottle, use filter to add chemical onto sample

## Patterning
**MLA**
* Prebake 
* Temp —> 110C 
* Time—> 60 s
* Let it cool down before putting in petrie dish
*  New Job 
* Exposure mode: series (does array)
* Load substrate: pneumatic / default
* 25x25 rectangular
* kLayouts file 
* HIMT —> designs —>gdsii
* Add .gds to filename 
* catpinholetest1.gds
* Design —> load converted klayout 
* New job ->> GDSII -> pick file
* Create default
* Expose mode: high quality 
* DMD width —> 1000 pixel is faster 
* Standard options —> none
* Center pattern in file
* Load substrate —> follow instructions on computer
* Parameters —> mode —> dose
* Array: use 55 fields, 6 rows, 50 mJ/cm^3 (7 steps), defoc -2, x/y step size -> 2mm
* Post bake
* Temp—-> 115C
* Time—> 60 s

**Develop**
* Fill beaker with AZ300MIF 
* Base
* Fully submerge + agitate sample in developer for 60 seconds
* Rinse with PW Water + dry with nitrogen air
* MF319 Waste bottle 
* Deposit Aluminum
* Tape samples to wafer

## Aluminium Deposition 
**Temescal  / electron beam evaporator**
* User: Pass:
* Automatic menu
* Auto menu-> vent pc (start)
* System map
* Unlatch when ready —> put sample in pc
* Auto menu—> pump pc 
* Up close (start)
* Auto menu —> recipe 
* Select folder 
* Standards —> Al.REC
* ~1 KA thick (100nm)
* Select recipe —> recipe (start)
* Data log -> name it
* Run log
* Start —> start recipe 
* Auto Control —> hold 
* Pauses deposit step 
* Resume when ready 
* Move beam around with remote to minimize power (evenly heat metal)—> save
* Automatically goes into vent step per recipe 
* Unlatch— > remove samples
* Auto menu —> pump PC
* Down open 
* Main —> log off

**Lift off**
* Sonic bath with acetone
* Time —> 5 mins

## Analysis 
**SEM**
* Image + characterize roughness 
* Vent chamber —> "air" (top right)
* Take sample to holder
* Specimen settings
* Following instructions
* Height of sample —> standard +2mm
* Diameter of sample —> ~50mm
* Enter size + height + "stage move"
* "Ok"
* *EVAC —> top right
*  Beep: HV on
*   Aperture —>  Condition
*    Check vacuum state
*    *HVAC ON —> top left
*    Condition -> electron beam
*    Vaca —> 5kV, 10 kV
* ABCC —> auto contrast
*  Done
*   High voltage —> off (top left)
*   Air —> top right
*   Open + take out sample + close door
*   EVAC —> top right 
