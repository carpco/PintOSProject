La carpeta pintos/src/ contiene el código original del SO que se va a modificar.

Las carpetas y una explicación de su contenido es:

	- devices: Esta carpeta contiene el código fuente para la interconexión de los dispositivos de entrada/salida: teclado,temporizador, 			   disco, etc.

	- filesys: Esta carpeta contiene el código fuente para un sistema de archivos básico.

	- lib: Esta carpeta contiene una implementación de un subconjunto de la biblioteca estandar de C. Tanto en el kernel de pinto, como en 		       los programas de usuario, los headers que contiene esta carpeta puden ser incluidos usando la notacion #include<...>.

	- misc:  

	- threads: 
	- userprog: 
	- utils: 
	- vm: 

Dentro de la carpeta threads/ encontramos los siguientes archivos:

	- flags.h:
	- init.c: 
	- interrupt.c: 
	- interrupt.h:
	- intr-stubs.h:
	- intr-stubs.S:
	- io.h:
	- kernel.lds.S:
	- loader.h:
	- loader.S:
	- Make.vars:
	- Makefile:
	- malloc.c:
	- malloc.h:
	- palloc.c:
	- palloc.h:
	- pte.h: 
	- start.S:
	- switch.h:
	- switch.S:
	- sync.c:
	- sync.h:
	- thread.c:
	- thread.h:
	- vaddr.h:

