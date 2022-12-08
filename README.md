# Vaja 8–I2C povezava z ADS1115 16-bit ADC pretv. terSTM32F0 Discovery
 
## Cilj naloge:

S pomočjo STM32CubeIDEin HAL knjižnicamisprogramirajte mikroprocesor tako, da bo preko I2C protokola prebral in prikazal analogne vrednosti iz 4-kanalnega ADC pretvornika ADS1115. Potrebujete tudi 4 trimerje/potenciometre, upore in kondenzator.Za prikaz spremenljivk potrebujete STMStudio(ali STM32CubeIDE v Debugnačinu).

## Postopek inicilizacije
- prizgeta se pina **PB7** in **PB6**.
- Omogoča **dve** različni komunikaciji.
- | ADS 1115: 	| SCL     	| SDA     	| ADDR                                                                 	| ALRT         	| VDD           	|
  |-----------	|---------	|---------	|----------------------------------------------------------------------	|--------------	|---------------	|
  | STM32F0:  	| **PB6** 	| **PB7** 	| Je povezan na GND Nato pa se preko<br> kondenzatorja(100nF) na +3.3V  	| (ni povezan) 	| 5 V ali 3.3 V 	|
- SDA in SCL sta povezna durg preg drugega z dvema 10kΩ med tema dvema uporamo je priključena napetost +3.3 V.
- Frekvvenca znaša 300KHz.


## Pinout

![Pinout](media/Screenshot_20221208_182220.png)

![](media\IMG_4676.MOV)

https://github.com/AV-35/Vaja8-I2C-ADS1115-STM32F0/blob/main/media/IMG_4676.MOV

https://github.com/AV-35/Vaja8-I2C-ADS1115-STM32F0/blob/a7ebb0321d8e0cdc02bc43049647f1918f14b24f/media/IMG_4676.MOV

media/IMG_4676.MOV
