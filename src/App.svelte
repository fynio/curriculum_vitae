<script>
  import { each } from "svelte/internal";

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
        
        redes_sociales:[
          {
            icono:"fab fa-facebook",
            url:"https://www.facebook.com/rodrigo.garciatrejo.965",
            title:"Facebook"
          },
          
          {
            icono:"fab fa-twitter",
            url:"https://twitter.com/Rodrigtoficial",
            title:"Twitter"
          }
          ,
          {
            icono:"fab fa-github",
            url:"https://github.com/fynio",
            title:"github"
          }
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
</script>

<style>
</style>

<main>
  <div class="container_cv">
    <div class="container_body">
      <div class="imagen_header">
        <img src="assets/images/fondo_arriba.svg?v=1" alt="" />
      </div>

      <div class="dividido">
        <div class="izq">
          <div class="contenedor">
            <div class="titulo_principal">Experiencia</div>

            {#each Data.persona[0].experiencia as item}
              <div class="contenedor_experiencia">
                <div class="lugar">{item.lugar}</div>
                <div class="puesto">{item.cargo}</div>
                <div class="fecha">{item.fecha}</div>
                <div class="descripcion">{item.descripcion}</div>
                <div class="tecnologia">{item.tecnologia}</div>
              </div>
            {/each}
          </div>

          <div class="contenedor_valores">
            <div class="titulo_principal">Skills</div>
            {#each Data.persona[0].skills as item}
              <div class="elemento">
                <div class="nombre">{item.nombre}</div>
                <div class="contenedor_estrellas">
                  {#if item.porcentaje >= 10}
                    {#each Array(item.porcentaje) as _, i}
                      <i class="fas fa-star " />
                    {/each}
                  {:else if item.porcentaje < 10}
                    {#each Array(item.porcentaje) as _, i}
                      <i class="fas fa-star " />
                    {/each}
                    {#each Array(10 - item.porcentaje) as _, i}
                      <i class="far fa-star " />
                    {/each}
                  {/if}
                </div>
              </div>
            {/each}
          </div>
        </div>

        <div class="centrado">
          <div class="contenedor_imagen">
            <div class="imagen">
              <img src="assets/images/foto.jpeg" alt="" />
            </div>
          </div>

          <!-- Aqui va el nombre -->
          <div class="nombre">
            {Data.persona[0].name}
          </div>

          <!-- Aqui va el puesto -->
          <div class="puesto">
            {Data.persona[0].perfil}
            </div>

          <div class="descripcion">{Data.persona[0].descripcion}</div>

          <div class="minicontenedor">
              <div class="titulo">

                Fecha de Nacimiento
              </div>
              <div class="descripcion">{Data.persona[0].fecha_nacimiento}</div>
    

          </div>

          <div class="minicontenedor">
            <div class="titulo">
              Dirección
            </div>
            <div class="descripcion">{Data.persona[0].estado}</div>
          </div>
        

          
          <div class="minicontenedor">
            <div class="titulo">
              Email
            </div>
            <div class="descripcion">{Data.persona[0].email}</div>
          </div>

           
          <div class="minicontenedor">
            <div class="titulo">
              Teléfono
            </div>
            <div class="descripcion">{Data.persona[0].telefono}</div>
          </div>

          
          <div class="minicontenedor">
            <div class="titulo">
              Página Web
            </div>
            <div class="descripcion">{Data.persona[0].pagina_web}</div>
          </div>

          <div>
            <br>
            <br>
            <br>
          </div>
          <div class="divisor">
            Redes Sociales
          </div>


          {#each Data.persona[0].redes_sociales as red_social}
          <div class="redes_sociales">
            <div>
              <a href="{red_social.url}" target="_black" title={red_social.title}>
                <i class="{red_social.icono}"></i>
              </a>
            </div>
          </div>
       
          {/each}


          <div class="wrapper">
            <div class="left triangle" />
            <div class="right triangle" />
          </div>
        </div>

        <div class="der">
          <div class="contenedor">
            <div class="titulo_principal">Educacion</div>

            {#each Data.persona[0].educacion as item}
              <div class="contenedor_experiencia">
                <div class="lugar">{item.lugar}</div>
                <div class="puesto">{item.cargo}</div>
                <div class="fecha">{item.fecha}</div>
              </div>
            {/each}
          </div>

          <div class="contenedor_valores">
            <div class="titulo_principal">Software</div>
            {#each Data.persona[0].software as item}
              <div class="elemento">
                <div class="nombre">{item.nombre}</div>
                <div class="contenedor_estrellas">
                  {#if item.porcentaje >= 10}
                    {#each Array(item.porcentaje) as _, i}
                      <i class="fas fa-star " />
                    {/each}
                  {:else if item.porcentaje < 10}
                    {#each Array(item.porcentaje) as _, i}
                      <i class="fas fa-star " />
                    {/each}
                    {#each Array(10 - item.porcentaje) as _, i}
                      <i class="far fa-star " />
                    {/each}
                  {/if}
                </div>
              </div>
            {/each}
          </div>
        </div>
      </div>
    </div>
  </div>
</main>
