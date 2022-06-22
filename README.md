# Pic 16F887 Salidas Digitales
<img src="https://github.com/IDiegoUlises/Pic-Salidas-Digitales/blob/main/Images/16f887-Pic.png"  />

* Vdd: Positivo del microcontrolador
* Vss: Negativo del microcontrolador
* Clkin: Osicilador conectado a negativo
* Clkout: Osicilador conectado a negativo


### Codigo
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

### Compilar en Css Compiler
<img src="https://github.com/IDiegoUlises/Pic-Salidas-Digitales/blob/main/Images/Codigo-Imagen.png"  />

### Conectar el Pic al Pickit 
<img src="https://github.com/IDiegoUlises/Pic-Salidas-Digitales/blob/main/Images/Pickit3.jpg" width="1000" height="500" />

### Subir el archivo Hex al Pickit 
<img src="https://github.com/IDiegoUlises/Pic-Salidas-Digitales/blob/main/Images/Importar-Hex.png"  />

### Luego subir el programa al microcontrolador con "Write"
<img src="https://github.com/IDiegoUlises/Pic-Salidas-Digitales/blob/main/Images/Write-pickit.png"  />

### Conexion
<img src="https://github.com/IDiegoUlises/Pic-Salidas-Digitales/blob/main/Images/Imagen-en-fritzing-3.png" />

