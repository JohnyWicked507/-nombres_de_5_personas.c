#include<stdio.h>
#include<conio.h>
typedef struct
{ char nombre[5]; // nombre y apellidos personas, jonathan sanches, maria lopez,cristian jr, nelson quintero, pedro castillo
 char dni[9]; // DNI
 int edad; // edad
 char sexo; // 'H' para hombre y 'M' para mujer
} DatosPersonales_t;
...
void main()
{
 DatosPersonales_t arrayDPersonales[5];
 int maxElem;
 ...
 // llamada a la funcion aquí:  nombre y apellidos personas, jonathan sanches, maria lopez,cristian jr, nelson quintero, pedro castillo
 ...
}
// Implementación de la funcion aquí:
Solución:
 // llamada a la funcion aquí:
 imprimeDatosPersonales(arrayDPersonales, maxElem);
// Implementación de la funcion aquí:
void imprimeDatosPersonales(DatosPersonales_t *datos, int elem)
{
 int i;
 for (i=0; i<elem; i++)
 {
 printf (“Nombre: %s, DNI: %s, EDAD: %d, SEXO: %c\n”,
 datos[i].nombre, datos[i].dni, datos[i].edad, datos[i].sexo);
 }
}
