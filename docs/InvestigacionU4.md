# ¿Qué es JSON y XML?  

## ¿Qué es JSON y para qué se Usa?  

Los datos son la clave. Sin embargo, saber cómo trabajar con diferentes datos es cada vez más importante. Los programadores, desarrolladores y profesionales de TI necesitan transferir estructuras de datos completas de cualquier idioma a formatos reconocibles por otros idiomas y plataformas. La notación de objetos JavaScript (JSON) es el formato de intercambio de datos que lo hace posible.  

JSON se convirtió en el formato de datos popular para los desarrolladores debido a su texto legible por humanos, que es liviano, requiere menos codificación y se procesa más rápido  

JSON se puede utilizar en programas JavaScript sin la necesidad de analizar o serializar. **Es una forma basada en texto para representar literales, matrices y datos escalar de objetos JavaScript**.  

JSON es relativamente fácil de leer y escribir y, además, es fácil de analizar y generar para el software. Se suele usar para serializar datos estructurados e intercambiarlos a través de una red, normalmente, entre un servidor y aplicaciones web.  

Si se lo analiza en detalle, JSON consta de tipos de datos.  

- Cadena
- Número
- Booleano
- Nulo
- Objeto
- Matriz

todos los textos deben estar entrecomillados con «comillas dobles», y solo se pueden utilizar tipos de datos como **string**,**number** ,**Object** ,**Array** ,**Boolean**  o **null**. Un valor null, simplemente, también sería un JSON válido.  

### **Ejemplos**  
Ejemplo de un objeto vacio
~~~
{
}
~~~
Ejemplo simple  pero entendible, haciendo una constante
~~~
const o = {
  name: "Manz",
  life: 99,
};
~~~
Ejemplo avanzado de varias constantes y con diferentes tipos de informacion que pueden almacenar  
~~~
{
  "name": "Manz",
  "life": 99,
  "dead": false,
  "props": ["invisibility", "coding", "happymood"],
  "senses": {
    "vision": 50,
    "audition": 75,
    "taste": 40,
    "smell": 50,
    "touch": 80
  }
}
~~~
### **Ventajas**  
- Es autodescriptivo y fácil de entender.  
- Su sencillez le ha permitido posicionarse como   alternativa a XML.  
- Es más rápido en cualquier navegador.  
- Es más fácil de leer que XML.  
- Es más ligero (bytes) en las transmisiones.  
- Se parsea más rápido.  
- Velocidad de procesamiento alta.  
- Puede ser entendido de forma nativa por los analizadores de JavaScript.  
### **Desventajas**  
- Algunos desarrolladores encuentran su escueta notación algo confusa.  
- No cuenta con una característica que posee XML: extensibilidad.  
- No soporta grandes cargas, solo datos comunes.  
- Para la seguridad requiere de mecanismos externos como expresiones regulares.  

## ¿Qúe es XML y para qué sirve?  
XML es un lenguaje de marcado similar a HTML. Significa Extensible Markup Language (Lenguaje de Marcado Extensible) y es una especificación de W3C como lenguaje de marcado de propósito general. Esto significa que, a diferencia de otros lenguajes de marcado, XML no está predefinido, por lo que debes definir tus propias etiquetas. **El propósito principal del lenguaje es compartir datos a través de diferentes sistemas, como Internet**.  

Hay muchos lenguajes basados en XML; Algunos ejemplos son XHTML, MathML, SVG, XUL, XBL, RSS, y RDF. También puedes crear uno propio.      

Para que un documento XML sea correcto, debe ser un documento bien formado, cumpliendo todas las reglas de sintaxis de XML, y válidas, acorde a las reglas de un lenguaje específico. Un ejemplo de un documento que no está bien formado es uno que tiene una etiqueta de apertura y no tiene una de cierre, ni se cierra en si misma.   
El lenguaje de marcado es un conjunto de códigos que se pueden aplicar en el análisis de datos o la lectura de textos creados por computadoras o personas. El lenguaje XML proporciona una plataforma para definir elementos para crear un formato y generar un lenguaje personalizado.  

Un archivo XML se divide en dos partes: prolog y body. La parte prolog consiste en metadatos administrativos, como declaración XML, instrucción de procesamiento opcional, declaración de tipo de documento y comentarios. La parte del body se compone de dos partes: estructural y de contenido (presente en los textos simples).  

El diseño XML se centra en la simplicidad, la generalidad y la facilidad de uso y, por lo tanto, se utiliza para varios servicios web. Tanto es así que hay sistemas destinados a ayudar en la definición de lenguajes basados ​​en XML, así como APIs que ayudan en el procesamiento de datos XML – que no deben confundirse con HTML.  

#### **Ejemplos**

 Esta es la forma incorrecta
~~~
 <message>
    <warning>
        Hola, mundo
    <!--missing </warning> -->
 </message>
~~~

Forma correcta  

~~~
<message>
    <warning>
         Hola, mundo
    </warning>
</message>
~~~

Usando entidades, este ejemplo es para mostrar un mensaje de "advertencia" 
~~~
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE body [
  <!ENTITY warning "Advertencia: Algo malo pasó... porfavor intente de nuevo.">
]>
<body>
  <message> &warning; </message>
</body>
~~~

### **Ventajas**
- Tiene un formato estructurado y fácil de comprender.  
- Separa radicalmente la información o el contenido de su presentación o formato.  
- Está diseñado para ser utilizado en cualquier lenguaje o alfabeto.  
- Su análisis sintáctico es fácil debido a las estrictas reglas que rigen la composición de un documento.  
- Tiene soporte a cualquier tipo de datos.  
- Se pueden definir estructuras complejas y reutilizables.  
### **Desventajas**
- El formato es sumamente estricto.  
- Lleva más tiempo procesarlo.  
- Complejidad de analizador (parser).  
- Un error en cualquier parte del formato puede hacer que todo el documento sea inválido.  


## **Comparando** 

|**JSON** | **XML**|
|-----|----|
|JSON es la notación de objetos de JavaScript| XML es el lenguaje de marcado extensible.|
|JSON se basa en el lenguaje JavaScript| XML se deriva de SGML.|
|JSON es una forma de representar objetos| XML es un lenguaje de marcado que utiliza una estructura de marcado para representar elementos de datos.|
|JSON no proporciona ningún soporte para espacios de nombres|XML admite espacios de nombres.|
|JSON admite matrices| XML no admite matrices.|
|los archivos JSON son muy fáciles de leer.|Los archivos XML son relativamente difíciles de leer e interpretarLos archivos XML son relativamente difíciles de leer e interpretar|
|JSON no utiliza etiquetas finales|XML tiene etiquetas de inicio y finalización.|
|JSON es menos seguro| XML es más seguro que JSON|
|JSON no admite comentarios |XML admite comentarios|
|JSON solo admite la codificación UTF-8 | XML admite varias codificaciones|

### *Fuentes*
- ¿Qué es JSON? (s. f.). ORACLE. Recuperado 17 de octubre de 2021, de <https://www.oracle.com/mx/database/what-is-json/>
- M.D.N. (2021, 16 octubre). Introducción a XML - XML: Extensible Markup Language | MDN. MDN Contributors. Recuperado 17 de octubre de 2021, de <https://developer.mozilla.org/es/docs/Web/XML/XML_introduction>
- Manz. (s. f.). JSON - Javascript en español. lenguajejs. Recuperado 17 de octubre de 2021, de <https://lenguajejs.com/javascript/caracteristicas/json/>
- Barrera, A. (2019, 10 noviembre). JSON: ¿Qué es y para qué sirve? NextU LATAM. Recuperado 17 de octubre de 2021, de <https://www.nextu.com/blog/que-es-json/>
- La diferencia entre JSON y XML - programador clic. (s. f.). programador clic. Recuperado 17 de octubre de 2021, de <https://programmerclick.com/article/60681955413/>
- de Souza, I. (2021, 12 febrero). XML: ¿qué es y para qué sirve este lenguaje de marcado? Rock Content - ES. Recuperado 17 de octubre de 2021, de <https://rockcontent.com/es/blog/que-es-xml/>