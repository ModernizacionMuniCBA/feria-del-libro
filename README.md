# Feria del libro
Aplicacion web/mobile con la agenda de la feria del libro.  

<p align="center">
  <img src="https://raw.githubusercontent.com/ModernizacionMuniCBA/feria-del-libro/gh-pages/www/res/screen-mobile-01.png" width="150"/>
  <img src="https://raw.githubusercontent.com/ModernizacionMuniCBA/feria-del-libro/gh-pages/www/res/screen-mobile-02.png" width="150"/>
  <img src="https://raw.githubusercontent.com/ModernizacionMuniCBA/feria-del-libro/gh-pages/www/res/screen-mobile-03.png" width="150"/>
</p>

Ya disponible en el [market de Android](https://play.google.com/store/apps/details?id=ar.gob.cordoba.gobiernoabierto.feriadellibro).    
Puede verse tambien [vía web](https://modernizacionmunicba.github.io/feria-del-libro) desde mobile.  

100% HTML5/JS con llamadas al [API de eventos de la Municipalidad de Córdoba](https://gobiernoabierto.cordoba.gob.ar/api/).  
Se usa como [web](https://modernizacionmunicba.github.io/feria-del-libro/) y embebida vía [Cordova](https://cordova.apache.org/) a aplicación Android.

Los datos están estructurados como:
 - Eventos: Agrupador principal. En este caso la _Feria del Libro_ es un evento que agrupa todo lo demás. 
 - Agrupador: Grupo de eventos relacionados. Para la feria del libro se definen _espacios_ que cumplirán este rol.
 - Actividades: Cada actividad en particular. 

Los datos sobre las llamadas API para cada objetos estan en [este documento](https://docs.google.com/document/d/1VuhbKmbkRHFx0L2HRRUuWv1HWqfk2LyCPOHAlIgq05g)

## Docs

Dejamos registrada la compilación de la app como instructivo en [2016](compilacion-2016.md) (sirvio para 2017) y la [2018](compilacion-2018.md).  

