# DIY-Geiger-Counter
**Homemade Geiger Counter and Dosimeter**

**1) GeigerPhone:**

GM Tubes:
- SBM20-1 GM tube with 0.3mm Lead foil for energy compensation: [GeigerPhone (Geiger Counter circuit) using LMC555](https://github.com/cyberelectronics/DIY-Geiger-Counter/blob/main/Pictures/SBM20_0.3mmLeadshield.jpg)
- [J401 (China) GM tube](https://github.com/cyberelectronics/DIY-Geiger-Counter/blob/main/Pictures/J305_GMtube.jpg)

This circuit can be connected to a smartphone (Android, iPhone – using [GeigerBot](https://sites.google.com/site/geigerbot/) with Jack adapter cable) or PC sound card (MIC IN).

Can be powered using one or two AA rechargeable or alkaline batteries.

The HV for the tube can be set with the  R3 trimmer.

[Circuit Schematic](https://github.com/cyberelectronics/DIY-Geiger-Counter/blob/main/Docu/GeigerPhone.pdf)

[Live Radiation Network by Radu](https://www.uradmonitor.com/)

**2) Geiger Counter using microcontroller:**

- [Video](https://youtu.be/5IWn8H0pbQ4)
- [Picture](https://github.com/cyberelectronics/DIY-Geiger-Counter/blob/main/Pictures/geiger.jpg)

The project details and firmware can be downloaded from [here](https://github.com/cyberelectronics/DIY-Geiger-Counter/tree/main/Docu).    

In this project I used a SBM20-1 GeigerMuller tube and an ATtiny2313 microcontroller.

This circuit can measure Gamma Dose Rate (GDR), Counts Per Minute (CPM) and Counts Per Second (CPS).

Also if you want you can connect to the PC for data logging, using this small free application available here:    [UGP](http://ea4eoz.blogspot.ro/2012/09/ugp-interfacing-geiger-tubes-to.html)

Then it is possible to import the values saved in a txt file (by UGP) to OpenOffice Calc and generate different charts:    [Chart Example](https://github.com/cyberelectronics/DIY-Geiger-Counter/blob/main/Docu/geiger.ods)

>[!NOTE]
>- Gamma Sensitivity for SBM20 tube is  29 cps/mR/h for Ra-226 and 22 cps/mR/h for Co-60
>- CPS to CPM conversion:    29 x 60 = 1740 CPM
>- Applying the absorbtion constant (8.77):    1740 / 8.77 = 198.4 cpm/uSv/h
>- Dose rate =  avgCPM / 198.4 = uSv/h
>
>OR
>- 1 cpm = 1 / 198.4 = 0.00504
>- Dose Rate =   avgCPM * 0.00504 = uSv/h
>
>For educational purposes only!

Thanks for conversion information to radiohobbystore.com




