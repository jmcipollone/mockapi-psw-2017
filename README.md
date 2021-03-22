# mockapi-psw-2017
Repositorio que se utiliza para definir un mock de la API de referencias requerida por los trabajos realizados durante el curso de Proyecto de Software

## Definición de la API de referencias
La API de referencias debe proveer los endpoints para recuperar tipos de documentos, obras sociales, tipos de vivienda, tipos de calefacción en una vivienda y tipos de agua en una vivienda.  Las URLs relativas para estos endpoints son las siguientes:
- /tipo-documento
- /obra-social
- /tipo-vivienda
- /tipo-calefaccion
- /tipo-agua

Por lo tanto, la API de referencias proporciona 5 tipos de recursos de información diferentes: tipos de documentos, obras sociales, tipos de viviendas, tipos de calefacción y tipos de agua. Por cada recurso de información (cualquiera sea su tipo) se registran dos propiedades:
id. Este atributo contiene un identificador numérico que identifica univocamente a un recurso de un determinado tipo.
nombre. Este atributo contiene una descripción textual de un recurso de un tipo determinado.

Los posibles recursos correspondientes a tipos de documentos son:
1. DNI
2. LC
3. LE
4. Pasaporte

Los posibles recursos correspondientes a obras sociales son:
1. IOMA
2. OSDE
3. Sancor

Los posibles recursos para tipos de vivienda son:
1. Material
2. Chapa
3. Adobe

Los posibles recursos para tipos de calefacción son:
1. Gas
2. Eléctrica
3. Leña

Los posibles recursos para tipos de agua son:
1. Corriente
2. Entubada

## Implementación del mock de la API de referencias
La versión "mock" o "fake" de la API de referencias se implementa usando "My JSON Server". Bajo esta herramienta, simplemente se realizaron los siguientes pasos para crear una versión mock de la API de referencias requerida por los sitios web desarrollados a lo largo del curso. Estos pasos son los siguientes:

I) Crear un repositorio público en GitHub correspondiente al mock de la API de referencias para el curso 2017 de Proyecto de Software. El repositorio creado se denominó de la siguiente manera: https://github.com/jmcipollone/mockapi-psw-2017

II) Crear un archivo "db.json" en el repositorio GitHub del punto 1. Este archivo contiene una colección de los diferentes tipos de recursos presentes en la API de referencias. El contenido de este archivo es:
```
  {
    "tipo-documento": [
      {
        "id": 1,
        "nombre": "DNI"
      }, ...
    ],
    "obra-social": [
      {
        "id": 1,
        "nombre": "IOMA"
      }, ...
    ],
    "tipo-vivienda": [
      {
        "id": 1,
        "nombre": "Material"
      }, ...
    ],
    "tipo-calefaccion": [
      {
        "id": 1,
        "nombre": "Gas"
      }, ...
    ],
    "tipo-agua": [
      {
        "id": 1,
        "nombre": "Corriente"
      }, ...
    ],
    ...
  }
```
III) Acceder a los recursos de la API de referencias mediante la siguiente URL: https://my-json-server.typicode.com/ \<github-user\> / \<github-repo\>
En nuestro caso particular, se reemplaza \<github-user\> con "jmcipollone" y se reemplaza \<github-repo\> con "mockapi-psw-2017", quedando la siguiente URL para la API de referencias: https://my-json-server.typicode.com/jmcipollone/mockapi-psw-2017.  

Algunos ejemplos:
- Para obtener la colección de obras sociales disponibles: https://my-json-server.typicode.com/jmcipollone/mockapi-psw-2017/obra-social
- Para obtener la obra social con ID 1: https://my-json-server.typicode.com/jmcipollone/mockapi-psw-2017/obra-social/1
