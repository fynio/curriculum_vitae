# Curriculum Vitae hecho con el framework Svelte

### Este repositorio lo comparto para que puedas crear tu curriculum vitae de una manera muy sencilla.

&nbsp;

## Fotografía

### Para modificar la fotografía ingresa a la carpeta ***public/images*** y remplaza la imagen ***foto.jpeg*** por tu fotografía.

&nbsp;

## Datos Personales  

### Para ingresar tus datos personales, lo único que tienen que hacer es modificar la constante Data que se encuentra en la carpeta ***src/App.svelte***, la cual es un objeto tipo JSON y está compuesto de la siguiente manera.

&nbsp;

``` json
  const Data = {
    persona: [
      {
        name: "Rodrigo Garcia Trejo",
        perfil: "Programador Web Fullstack",
        descripcion:
          "Programador creativo y analítico, capaz de realizar aplicativos eficientes y eficaces, acostumbrado a trabajar bajo presión y capaz de resolver problemas a través del uso de la tecnología web.",
        fecha_nacimiento: "22-10-1989",
        estado: "Actopan Hidalgo, México",
        email: "rodrigogarciatrejo89@gmail.com",
        telefono: "7721065676",
        pagina_web: "rodrigogarciatrejo89.com.mx",
        redes_sociales: [
          {
            icono: "fab fa-facebook",
            url: "https://www.facebook.com/rodrigo.garciatrejo.965",
            title: "Facebook",
          },

          {
            icono: "fab fa-twitter",
            url: "https://twitter.com/Rodrigtoficial",
            title: "Twitter",
          },
        ],

        experiencia: [
          {
            lugar: "Sistema Nacional DIF",
            cargo: "Programador Técnico",
            fecha: "Febrero - Junio 2015",
            descripcion:
              "Crear una página web en Asp.net con conexión a una base de datos hecha en SQL Server utilizando Ajax donde implemente bootstrap, CSS, JavaScript y gráficas para un Cubo OLAP que se pretende implementar en el departamento de Dirección de Planeación y Evaluación del sistema Dif Hidalgo",
            tecnologia:
              "SQL Server, Boostrap, CSS, jS, JQuery, ASP.net con IIS",
          },
        ],
        educacion: [
          {
            lugar: "Universidad Autonoma del Estado de Hidalgo",
            cargo: "Licenciatura en Sistemas Computacionales",
            fecha: "2009 - 2015",
          },
          {
            lugar: "Universidad de Cádiz",
            cargo:
              "Diplomado en Estrategias y Prevención de Crímenes Digitales",
            fecha: "Noviembre 2018",
          },
        ],
        software: [
          {
            nombre: "Javascript",
            porcentaje: 8,
          },
          {
            nombre: "Jquery",
            porcentaje: 9,
          },
        ],

        skills: [
          {
            nombre: "Comunicación",
            porcentaje: 8,
          },
          {
            nombre: "Sencilles",
            porcentaje: 9,
          },
        ],
      },
    ],
  };
```




&nbsp;
## Datos Generales

### En está primera parte debe ingresar sus datos personales:
### ***Nombre***: Nombre completo.
### ***Perfil***: Carrera profesional o ultimo grado de estudios.
### ***Descripción***: Describe tu perfil profesional, ejemplo: Programador FullStack.
### ***Estado***: Estado al que perteneces.
### ***Teléfono***.
### ***Email***.
### ***Página Web***.

&nbsp;
&nbsp;
## Skills y Software
&nbsp;
### En esta sección necesitas ingresar un porcentaje solo debes ingresar un valor entre 1-10 el cual representa su nivel en el manejo del Software o del Skills, Puede ingresar tantos elementos de Skills y Software necesite.
&nbsp;

```json
    {
        nombre: "TypeScript",
        porcentaje: 6,
    },
```

&nbsp;
## Redes Sociales
### En esta sección necesita un icono, una url y un title. 
### Icono: ingresar el nombre del icono, el cual podrás elegir en el siguiente link [Font-Awesome](https://fontawesome.com/icons?d=gallery) y colocar el nombre de la clase, por ejemplo: para el icono de twiiter "fab fa-twitter" . 
### Url: ingresar el link de su red social, ejemplo: "https://github.com/fynio". 
### Title: ingresar una pequeña descripción sobre el enlace.
&nbsp;

```json
    {
        icono: "fab fa-github",
        url: "https://github.com/fynio",
        title: "github",
    },
```
&nbsp;
## Si configuró todo correctamente, deberá ver una página similar a esta => [Ver Curriculum](https://distracted-hamilton-2c2349.netlify.app/).

&nbsp;
### ¡¡Muchas gracias por su atencion!!