# Arduino fan emulator

### 📌 Part list
✔ Arduino Nano ( or  any other based on 328p)  
✔ 1 * 10K resistor  
✔ 1 * 1K resistor  
✔ 1 * npn 2n222* transistor  
✔ wires, connectors  

Upload code to arduino via [Arduino IDE](https://www.arduino.cc/en/Main/Software)

### 📌 Arduino is powered from fan terminal directly
🔌 Black is GND  
🔌 Red is +12V  
🔌 Yellow wire - PG (usualy 3rd is fan output that we are going to emulate).

> 1️⃣ You need to connect +12V to VIN pin of Arduino, and GND to GND pin.  
> 2️⃣ 2n222 collector should be connected to +12V (or +5v if there is no way to get 12v) through 10K resistor  
> 3️⃣ 2n222 base should be connected to D9 through 1K resistor  
> 4️⃣ 2n222 emitter should be connected to GND  
> 5️⃣ Output signal will be generated between 10R resistor and collector.

![Scheme](https://github.com/kofbox/Antminer-fan-emulator-fork/blob/master/Scheme.png)
