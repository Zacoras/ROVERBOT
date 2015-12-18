# ROVERBOT
Proyecto de robot usando: STM32F411, plataforma ROVER5, MBED, MPU6050
Hola soy Derick
Oppa Gangna Style tururu tururur chuchuchu pa
Para este proyecto se emplea una tarjeta STM32F411RET6(Nucleo F411), junto con MBED para una fácil programacion además de algunos sensores,motores, puentes H, todo montado sobre una plataforma ROVER 5. 
# Requisitos
	 gcc-arm-embedded: https://launchpad.net/gcc-arm-embedded
	 make: apt-get install make o yum install make
	 st-link: https://github.com/texane/stlink

#Instalación
En el archivo Makefile editar las lineas ST_LINK, GCC_BIN y colocar las rutas donde se encuentren los binarios correspondientes.

	ST_LINK hace referencia a donde esta instalado st-link(requisito).
	GCC_BIN hace refetencia a donde esta la carpeta bin del compilador gcc-arm-embedded.
	
En caso de que hayan sido agregados a la variable de sistema PATH, con el comando whereis o which desde la consola pueden obtener las rutas.

	whereis st-link
	which arm-none-eabi-gcc

#Compilación
	make

#Subir a la targeta
	make upload

#Limpiar build
	make clean
