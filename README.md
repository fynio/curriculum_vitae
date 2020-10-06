# Curriculum Vitae hecho con el framework Svelte

### Esta diseñado para que pueden utilizarlo y modificar el archivo json para que ingresen sus datos personales.

&nbsp;

## Opciones

&nbsp;

## Fotografía

### Para modificar la fotografía ingresen a la carpeta public/images/foto.jpeg

&nbsp;

## Datos Personales

### Para ingresar sus datos personales, lo único que tienen que hacer es modificar la constante Data que se encuentra en la carpeta src/App.svelte

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
          {
            icono: "fab fa-github",
            url: "https://github.com/fynio",
            title: "github",
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
          {
            lugar: "Subsecretaría de Inversiones y Productividad Sectorial",
            cargo: "Programador FullStack",
            fecha: "Octubre - Diciembre 2016",
            descripcion:
              "Crear página web para atraer inversiónes al estado de Hidalgo",
            tecnologia:
              "Boostrap, CSS, JS, JQuery, MySQL en un servidor tipo LAMP",
          },
          {
            lugar: "Subsecretaría de Fomento Económico",
            cargo: "Programador FullStack",
            fecha: "Mayo 2018 - Actualidad",
            descripcion:
              "Crear diferentes Plataformas comó Mi Primer Empleo, Consume Hidalgo, CRM Empresarial, Expofinanciamiento",
            tecnologia:
              "React, Vue, Angular, PHP, Boostrap, CSS, JS, JQuery, MySQL, Postgres",
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

          {
            nombre: "Php",
            porcentaje: 9,
          },

          {
            nombre: "React",
            porcentaje: 8,
          },

          {
            nombre: "Vue",
            porcentaje: 8,
          },

          {
            nombre: "Angular",
            porcentaje: 7,
          },

          {
            nombre: "Django",
            porcentaje: 6,
          },

          {
            nombre: "NodeJs",
            porcentaje: 8,
          },

          {
            nombre: "Svelte",
            porcentaje: 6,
          },

          {
            nombre: "TypeScript",
            porcentaje: 6,
          },

          {
            nombre: "Css",
            porcentaje: 9,
          },

          {
            nombre: "Sass",
            porcentaje: 8,
          },

          {
            nombre: "HTML",
            porcentaje: 9,
          },

          {
            nombre: "Bootstrap",
            porcentaje: 9,
          },

          {
            nombre: "Materialize",
            porcentaje: 9,
          },

          {
            nombre: "SemanticUI",
            porcentaje: 9,
          },

          {
            nombre: "Java",
            porcentaje: 7,
          },

          {
            nombre: "Laravel",
            porcentaje: 0,
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

          {
            nombre: "Honestidad",
            porcentaje: 10,
          },

          {
            nombre: "Franqueza",
            porcentaje: 10,
          },

          {
            nombre: "Trabajo en Equipo",
            porcentaje: 10,
          },

          {
            nombre: "Amabilidad",
            porcentaje: 10,
          },

          {
            nombre: "Creatividad",
            porcentaje: 10,
          },

          {
            nombre: "Dedicación",
            porcentaje: 10,
          },

          {
            nombre: "Resolución de Problemas",
            porcentaje: 10,
          },

          {
            nombre: "Colaboración",
            porcentaje: 10,
          },
        ],
      },
    ],
  };
```


## Skills y Software
&nbsp;
### En esta sección pide un porcentaje solo permiete ingresar del 1-10 donde deberán ingresar el porcentaje de manejo del Software o del Skill, pueden la cantidad de skills o software que necesiten
&nbsp;

```json
    {
        nombre: "TypeScript",
        porcentaje: 6,
    },
```

&nbsp;
## Redes Sociales
&nbsp;
### En esta sección necesita un icono, una url y un title. 
### En icono deberan ingresar un icono de [Font-Awesome](https://fontawesome.com/icons?d=gallery) 
### En url deben ingresar la url de su red social
### En title es el titulo de la red social esto solo para que salga una descripción de la red social.
&nbsp;

```json
    {
        icono: "fab fa-github",
        url: "https://github.com/fynio",
        title: "github",
    },
```

  