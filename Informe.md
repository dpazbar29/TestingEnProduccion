# INFORME TÉCNICO

## 1. EVALUACIÓN INICIAL DE ESTÁNDARES Y NAVEGACIÓN
### ELECCIÓN DE PROYECTO
El proyecto seleccionado finalmente ha sido el mío mismo, ya que al conocerlo completamente puedo realizar un análisis más prfundo.

### ANÁLISIS DE LOS ESTÁNDARES EMPLEADOS EN EL DESARROLLO
Trataré 5 tipos de stándares, **ACCESIBILIDAD** *(WCAG, ARIA)*, **CÓDIGO Y SEMÁNTICA WEB** *(HTML, CSS, JavaScript)*, **USABILIDAD**, **RENDIMIENTO** *(velocidad de carga, SEO)* y **COMPATIBILIDAD**.

#### **ACCESIBILIDAD**
##### WCAG
Tras realizar un análisis de nivel AA, podemos encontrar bastantes errores como: 
- Controles de formulario sin etiquetar
- Imágenes sin descripción
- Etiquetas como h1 no utilizadas dando problemas con lecturas de página web para usuarios que padecen ceguera
- Idioma no declarado

[Enlace a los resultados del test](/InformeWCAG.md)

##### ARIA
No hay ningún uso de ARIA

#### **ESTÁNDARES DE CÓDIGO Y SEMÁNTICA WEB**
##### HTML
Tras analizar mi página con *W3C HTML Validator* no obtengo ningún error ni advertencia respecto a la estructura HTML, todas las etiquetas están bien colocadas y cerradas.

##### CSS
También he analizado mi CSS con *W3C CSS Validator* y tampoco se ha encontrado ningún error.

#### **ESTÁNDARES DE USABILIDAD**
La navegación es intuitiva, el diseño es en cierta manera responsivo, aunque en ciertos tamaños da fallos con el tamaño de algunos elementos, los botones son claros y los formularios son intuitivos

### TESTS 

#### **WebPageTest**
Cada test ha sido realizado en más de una ocasión, para así analizar la media de estos.
- **Chrome**: el home en este navegador carga rápidamente, tarda un segundo en aparecer los primeros pixeles y el contenido de la página aparece milésimas antes de la imágen y al momento que la página termina de cargar ya es usable, además de esto, la página no varió, ni se bloqueó en ningún momento durante la carga. 

![Test en Chrome](/Recursos/TestChrome.jpg)

- **Firefox**: el home en este caso empezó a cargar al medio segundo (casi 5 veces más lento que con Chrome), los primeros pixeles aparecieron casi a los 2 segundos, poco después las imágenes y tardó 1.8 segundos en ser usable, además la página no se bloqueó durante la carga.

![Test en Firefox](/Recursos/TestFirefox.jpg)

Debido a problemas con mi despliegue al parecer no es posbile analizar paginas que no sean el home ya que la página no las reconoce.

- **Chrome(móvil 4G)**: el home carga de manera lenta pero aun así aceptable, la página es usable al cabo de casi 4 segundos, y al rededor de los 3,5 segundos es cuando empieza a cargarse la página, esta vez la página si se ha bloqueado en algún momento y ha cambiado durante la carga un 0.001.

![Test Chrome Móvil 4G](/Recursos/ChromeMovil4G.jpg)

- **Chrome(móvil 3G)**: en este caso, el home carga 1 segundo más tarde que en el otro móvil y tardó al rededor de 5 segundos y medio en ser usable, pasando a números malos, aun así también solo cambió el diseño 0.001 veces y se bloqueó durante 0.150 segundos.

![Test Chrome Móvil 3G](/Recursos/ChromeMovil3G.jpg)

#### **PageSpeed Insights**
De la misma manera que con la página anterior, solo podré hacer las pruebas con el home.

- **Móvil**:
El rendimiento es medio-bajo, con un puntaje de 66, la accesibilidad es media-alta con un 85, el puntaje de prácticas recomendadas es de 100 y el SEO 91.

![Test Móvil Speed](/Recursos/TestSpeedMovil.jpg)

El renderizado del mayor elemento es lento, existen elementos que bloquean el renderizado, hay contenido de JavaScript, el tamaño de algunas imágenes no es adecuado.

Además debería evitar cambios de diseño importantes, el tiempo de respuesta es breve

- **Ordenador**: 
El rendimiento es excelente, con 99 puntos, mejorando mucho respecto al móvil, la accesibilidad, las prácticas recomendadas y el SEO se mantienen igual.

![Test Ordenador Speed](/Recursos/TestSpeedPc.jpg)

### EVALUACIÓN CON GHOST INSPECTOR
Respecto al test de prueba, funciona según lo esperado, el test se ha realizado a la perfección completamente y con una velocidad de respuesta adecuada.

[Enlace al vídeo del test](./Recursos/VideoGhost.mp4)
