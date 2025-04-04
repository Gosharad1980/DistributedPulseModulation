# DistributedPulseModulation

Distributed pulse modulation done like with the old P82C150, but with descrete components

## "Theory of operation"

Au lieu de grouper tous les pulse de fançon contigüe comme en PWM, le principe est de les distribuer le plus uniformément possible sur a période du compteur.

### Sur la base du P82C150
[P82C150 - Application note](https://www.nxp.com/docs/en/application-note/AN94088.pdf)

[P82C150 datasheet](https://www.digchip.com/datasheets/parts/datasheet/364/P82C150AHT-pdf.php)

![DDPM-P82C150](./img/DDPM-P82C150.jpg)

### Sur la base de la thèse de Paolo S. Crovetti
[Thèse : Paolo S. Crovetti](https://www.researchgate.net/publication/309012492_All-Digital_High_Resolution_DA_Conversion_by_Dyadic_Digital_Pulse_Modulation)

![DDPM-SPDT-4bits-pattern](./img/DDPM-SPDT-4bits-pattern.jpg)


## La carte de développement

Permet de faire :
* PWM (Pulse Width Modulation)
* DPM façon P82C150 (Distributed Pulse Modulation)
* DDPM (Dyadic Discrete Pulse Modulation)

### PWM

* ne pas monter les CD74HCT4053
* positionner les jumpers comme dans le schéma (PWM/DDPM) sérigraphié sur le PCB
![P82C150_PWM](./img/P82C150_PWM.png)

### DPM

* ne pas monter les CD74HCT4053
* positionner les jumpers comme dans le schéma (DPM) sérigraphié sur le PCB
![P82C150_DPM](./img/P82C150_DPM.png)

### DDPM

* ne pas monter les 74LS85
* positionner les jumpers comme dans le schéma (PWM/DDPM) sérigraphié sur le PCB
![Dyadic_Discret_Pulse_Modulation](./img/Dyadic_Discret_Pulse_Modulation.png)