# Pic 16F887 Salidas Digitales
<img src="https://github.com/IDiegoUlises/Pic-Hola-Mundo/blob/main/Images/16f887-Pic.png"  />

* Vdd: Positivo del microcontrolador 
* Vss: Negativo del microcontrolador
* Clkin: Osicilador a conectado negativo
* Clkout: Osicilador a conectado negativo

<img src="https://github.com/IDiegoUlises/Pic-Hola-Mundo/blob/main/Images/Codigo-Imagen.png"  />

```c
#include <16f887.h> //Nombre del microcontrolador
#fuses xt,nowdt  //para osciladores de 4 MegaHertz se usa xt para mayores usa hs
#use delay(clock=4M) //Velocidad del oscilador, la "M" signfica mega

void main()
{
   while(true)
   {
      output_high(pin_c0); //Enciende el led
      delay_ms(1000); //Espera de 1 segundo
      output_low(pin_c0); //Apaga el led
      delay_ms(1000); //Espera de 1 segundo
   }
}

```
