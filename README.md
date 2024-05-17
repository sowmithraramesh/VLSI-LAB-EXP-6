# SCHEMATIC AND SIMULATION OF CMOS INVERTER,NOR AND NAND GATE USING CADENCE virtuoso

## AIM:
     To design the following circuits using Cadence Virtuoso
     1) Inverter
     2) 2 Input NAND gate
     3) 2 Input NOR gate

## SOFTWARE REQUIRED: 
              Cadence Virtuoso
## PROCEDURE
 #### Commands to get into Cadence
   1.Right Click and open the terminal window
   2.Type the following commands as follows and press enter.
   i)tcsh
   ii)source /home/install/cshrc
   iii)virtuoso
 #### Procedure for Schematic simulation using Cadence
   1.Now two windows must open i)virtuoso/command interpreter window 
   ii)”Whats New…”
   2.Close the 2nd window
   3.Use 1st window i.e virtuoso window(CIW) for further processing.
   i)Create a New Library
   ii)Create Schematic Cell view.
   iii)Create the Symbol for schematic Cell view.
   iv)Create the test Cell view.
   v)Analog simulation by spectre
 #### Procedure for Creating New Library.
   a)File –New – Library
   b)Name : Give name for ur library Ex: VLSILAB , Enable Attach to an existing
   technology library, Click OK
#### Create Schematic Cell view.
   a)Go to 1st window i.e virtuoso(CIW)
   b)File-New-Cell view
   c)Setup the new file form, Library: Select the one you a created. Cell : Give the
    experiment name Ex: Inverter View: Schematic
   d)Type: Schematic press OK
   e)Add the required components from the libraries and make the connections.
   f)Go to instance fixed menu or use shortcut key “I” from keypad to go instances
   Click on browse. This opens the library browser ow select the appropriate library for
   components like Gpdk045,nmos, pmos
   g)Analog library Vdd, Gnd, Vcc, Vpulse, Vsin
   h)Make the connections by using fixed narrow wire key
    i)Click Check and Save button
#### Creating the Symbol for schematic Cell view
   a.In the schematic window, execute
   Crate – Cell view – From Cell view
   The cell view from cell view window appears
   Check Lib Name, Cell Name, From View name must be schematic Press ok
   b.Now Symbol generation form appears. Click Ok If No changes required
   c.A new window with with default symbol is created.
   d.Edit the symbol if you want to give actual symbol shape else continue.
   i.Execute Create-Cell view-from cell view
   ii.Library Name and Cell Name must be same which you have used for
   schematic. Press OK
   iii.Check for the position of pin side.Prss OK
   iv.Edit for the shape by Create-Shape-Choose required options to edit.
  #### Creating the new test cell view
   a)Go to CIW window, Execute File-New-Cell view
   b)Setup the new file form
   Library: Select the one you a created.
   Cell: Cell name must be different from the name used in schematic cell view.
   Ex: Inverter_test
   View: Schematic
   Type: Schematic press OK
#### Analog simulation by SPECTRE.
   a.In test cell view window
   i.Launch – ADE L(Analog Design Environment)
   b.Execute Setup—Simulation/directory/Host A new window opens
   c.Set the simulation window to spectre and click ok
   d.Execute Setup-Model Library. Anew window opens, Check of gpdk.scs as lib and
   section type as stat then press OK.
   e.Execute Analysis – Choose. A window opens.
   f.Select the type and set the specifications and press OK
   g.Execute Output s—to be plotted – Select on Schematic
   h.Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test
#### Schematic using mouse
   i.Execute Simulation -- Net list and Run

## CMOS INVERTER SCHEMATIC:
![image](https://github.com/sowmithraramesh/VLSI-LAB-EXP-6/assets/166893766/4211df6f-9187-4877-9ac5-5170246ffc12)
![image](https://github.com/sowmithraramesh/VLSI-LAB-EXP-6/assets/166893766/64f745c7-2b7d-42fe-af7d-b8089d38972f)

### SPECIFICATIONS
    Vpulse V1 = 0, V2 = 1
    Vdc = 1
    td = 0,tr = tf = 1 n, ton = 100n ,T = 200n
### OUTPUT:
Simulation Settings
Setup for transient analysis:
    1.Stop time = 400n
Setup for D.C analysis
    1.Component to be selected in schematic is for d.c analysis
    2.Start = -1 Stop = 1 resp.

### TRANSIENT ANALYSIS
![image](https://github.com/sowmithraramesh/VLSI-LAB-EXP-6/assets/166893766/c2f5bbcc-ae7c-4d45-83ee-18371d275c7d)

### DC ANALYSIS
![image](https://github.com/sowmithraramesh/VLSI-LAB-EXP-6/assets/166893766/d483c6ec-4879-4113-8b33-22055a9267df)

## 2 INPUT NAND:
![image](https://github.com/sowmithraramesh/VLSI-LAB-EXP-6/assets/166893766/a27e358d-d812-4368-a12c-c4cdefa7cffc)
![image](https://github.com/sowmithraramesh/VLSI-LAB-EXP-6/assets/166893766/f41b0a60-e25c-42d8-95d0-3f8ac054d2b9)

### SPECIFICATIONS
    Vpulse A V1 = 0, V2 = 1,Vpulse B V1 = 0, V2 = 1
    Vdc = 1
    For Vpulse A td = 0,tr = tf = 1 n, ton = 200n ,T = 100n
    For Vpulse B td = 0,tr = tf = 1 n, ton = 100n ,T = 50n

### OUTPUT: 
Simulation Settings
Setup for transient analysis:
    1.Stop time =400n
![image](https://github.com/sowmithraramesh/VLSI-LAB-EXP-6/assets/166893766/d426286d-5c11-40c9-8c5e-216810c77ee7)

## 2 INPUT NOR:
![image](https://github.com/sowmithraramesh/VLSI-LAB-EXP-6/assets/166893766/f1f317fb-33bc-47ce-ad0c-d3514727fd8a)
![image](https://github.com/sowmithraramesh/VLSI-LAB-EXP-6/assets/166893766/e0737a75-0805-448f-b6d2-9bf2b5c925fc)

### SPECIFICATIONS
    Vpulse A V1 = 0, V2 = 1,Vpulse B V1 = 0, V2 = 1
    Vdc = 1
    For Vpulse A td = 0,tr = tf = 1 n, ton = 200n ,T = 100n
    For Vpulse B td = 0,tr = tf = 1 n, ton = 100n ,T = 50n
### OUTPUT: 
     Simulation Settings
     Setup for transient analysis:
     1.Stop time =400n
     ![image](https://github.com/sowmithraramesh/VLSI-LAB-EXP-6/assets/166893766/7e70514f-c0bf-4a3d-a8be-74e6942a07df)

## RESULT:
     The schematic and simulate inverter using CADENCE is done and verified successfully.
    




   

   

