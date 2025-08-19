<!--  <div class="row mt-5">
        <div class="col-md-4">
          <div class="card h-100 bg-light shadow">
            <img src="image4.jpg" class="card-img-top" alt="Medicina">
            <div class="card-body">
              <h5 class="card-title">Medicine for Poor Children</h5>
              <p class="card-text">Lorem ipsum dolor sit amet consectetur adipiscing elit.</p>
              <a href="#" class="btn btn-primary">Learn More</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card h-100 bg-light shadow">
            <img src="image5.jpg" class="card-img-top" alt="Help">
            <div class="card-body">
              <h5 class="card-title">Help for Children of the East</h5>
              <p class="card-text">Lorem ipsum dolor sit amet consectetur adipiscing elit.</p>
              <a href="#" class="btn btn-primary">Learn More</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card h-100 bg-light shadow">
            <img src="image6.jpg" class="card-img-top" alt="Youth">
            <div class="card-body">
              <h5 class="card-title">Youth in the Communities of Medellín</h5>
              <p class="card-text">Lorem ipsum dolor sit amet consectetur adipiscing elit.</p>
              <a href="#" class="btn btn-primary">Learn More</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
 -->


 <!-- videocar -->
 <!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Carousel con Videos</title>
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css"
      rel="stylesheet"
    />
    <style>
      .carousel-item video {
        width: 100%;
        height: auto;
      }
    </style>
  </head>
  <body>
    <div id="videoCarousel" class="carousel slide" data-bs-ride="carousel">
      <div class="carousel-inner">
        <div class="carousel-item active">
          <video class="d-block w-100" muted>
            <source src="../recursos/videos/1 min's instagram 2025-2-20 story.mp4" type="video/mp4" />
          </video>
        </div>
        <div class="carousel-item">
          <video class="d-block w-100" muted>
            <source src="../recursos/videos/1 min's instagram 2025-2-20 story.mp4" type="video/mp4" />
          </video>
        </div>
        <div class="carousel-item">
          <video class="d-block w-100" muted>
            <source src="../recursos/videos/Huellas de barrio Un abrazo fraterno y amoroso a los barrios populares - LILIANA MARIA SANCHEZ MAZO (1080p, h264).mp4" type="video/mp4" />
          </video>
        </div>
      </div>
      <button
        class="carousel-control-prev"
        type="button"
        data-bs-target="#videoCarousel"
        data-bs-slide="prev"
      >
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      </button>
      <button
        class="carousel-control-next"
        type="button"
        data-bs-target="#videoCarousel"
        data-bs-slide="next"
      >
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
      </button>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script>
      const carousel = document.getElementById('videoCarousel');
      const videos = carousel.querySelectorAll('video');

      carousel.addEventListener('slid.bs.carousel', (event) => {
        videos.forEach((video) => video.pause()); // Pausar todos los videos
        const activeVideo = event.relatedTarget.querySelector('video');
        if (activeVideo) {
          activeVideo.play(); // Reproducir solo el video activo
        }
      });
    </script>
  </body>
</html>





 <div id="videoCarousel" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-inner">
            <div class="carousel-item active">
                <video class="d-block w-100" muted>
                    <source src="video1.mp4" type="video/mp4">
                </video>
                <button class="sound-toggle">🔊</button>
            </div>
            <div class="carousel-item">
                <video class="d-block w-100" muted>
                    <source src="video2.mp4" type="video/mp4">
                </video>
                <button class="sound-toggle">🔊</button>
            </div>
            <div class="carousel-item">
                <video class="d-block w-100" muted>
                    <source src="video3.mp4" type="video/mp4">
                </video>
                <button class="sound-toggle">🔊</button>
            </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#videoCarousel" data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#videoCarousel" data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
        </button>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script>
        const carousel = document.getElementById('videoCarousel');
        const videos = carousel.querySelectorAll('video');
        const buttons = document.querySelectorAll('.sound-toggle');

        carousel.addEventListener('slid.bs.carousel', event => {
            videos.forEach(video => video.pause()); // Pausar todos los videos
            const activeVideo = event.relatedTarget.querySelector('video');
            if (activeVideo) {
                activeVideo.play(); // Reproducir solo el video activo
            }
        });

        buttons.forEach(button => {
            button.addEventListener('click', event => {
                const video = event.target.previousElementSibling;
                if (video.muted) {
                    video.muted = false;
                    event.target.textContent = '🔇';
                } else {
                    video.muted = true;
                    event.target.textContent = '🔊';
                }
            });
        });
    </script>


  img
  
    https://lamemoriaseconstruyecaminando.wordpress.com/wp-content/uploads/2017/02/dsc4533-editar-5.jpg?w=648


    https://github.com/Sektor30/dise-oProyecto3/blob/main/assets/up2.png?raw=true


    

    acoordeon

    <li>
              <div class="accordion" id="accordionExample">
                <div class="accordion-item">
                  <h2 class="accordion-header" id="headingOne">
                    <button
                      class="accordion-button"
                      type="button"
                      data-bs-toggle="collapse"
                      data-bs-target="#collapseOne"
                      aria-expanded="true"
                      aria-controls="collapseOne"
                    >
                      Accordion Item #1
                    </button>
                  </h2>
                  <div
                    id="collapseOne"
                    class="accordion-collapse collapse "
                    aria-labelledby="headingOne"
                    data-bs-parent="#accordionExample"
                  >
                    <div class="accordion-body">
                      <strong>This is the first item's accordion body.</strong>
                      It is shown by default, until the collapse plugin adds the
                      appropriate classes that we use to style each element.
                    </div>
                  </div>
                </div>
                <div class="accordion-item">
                  <h2 class="accordion-header" id="headingTwo">
                    <button
                      class="accordion-button collapsed"
                      type="button"
                      data-bs-toggle="collapse"
                      data-bs-target="#collapseTwo"
                      aria-expanded="false"
                      aria-controls="collapseTwo"
                    >
                      Accordion Item #2
                    </button>
                  </h2>
                  <div
                    id="collapseTwo"
                    class="accordion-collapse collapse"
                    aria-labelledby="headingTwo"
                    data-bs-parent="#accordionExample"
                  >
                    <div class="accordion-body">
                      <strong>This is the second item's accordion body.</strong>
                      It is hidden by default, until the collapse plugin adds
                      the appropriate classes that we use to style each element.
                      These classes control the overall appearance, as well as
                      the showing and hiding via CSS transitions. You can modify
                      any of this with custom CSS or overriding our default
                      variables. It's also worth noting that just about any HTML
                      can go within the <code>.accordion-body</code>, though the
                      transition does limit overflow.
                    </div>
                  </div>
                </div>
                <div class="accordion-item">
                  <h2 class="accordion-header" id="headingThree">
                    <button
                      class="accordion-button collapsed"
                      type="button"
                      data-bs-toggle="collapse"
                      data-bs-target="#collapseThree"
                      aria-expanded="false"
                      aria-controls="collapseThree"
                    >
                      Accordion Item #3
                    </button>
                  </h2>
                  <div
                    id="collapseThree"
                    class="accordion-collapse collapse"
                    aria-labelledby="headingThree"
                    data-bs-parent="#accordionExample"
                  >
                    <div class="accordion-body">
                      <strong>This is the third item's accordion body.</strong>
                      It is hidden by default, until the collapse plugin adds
                      the appropriate classes that we use to style each element.
                      These classes control the overall appearance, as well as
                      the showing and hiding via CSS transitions. You can modify
                      any of this with custom CSS or overriding our default
                      variables. It's also worth noting that just about any HTML
                      can go within the <code>.accordion-body</code>, though the
                      transition does limit overflow.
                    </div>
                  </div>
                </div>
              </div>
            </li>





            dropdown simple


             <li>
              <div class="btn-group">
                <button class=" dropdown-toggle"  id="dropdownMenuButton" data-bs-toggle="dropdown" aria-expanded="false">
                  Dropdown
                </button>
                <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton">
                  <li><a class="dropdown-item" href="#">investigacion</a></li>
                  <li><a class="dropdown-item" href="#">formacion</a></li>
                  <li><a class="dropdown-item" href="#">educacion</a></li>
                </ul>
              </div>
            </li>



            antiguo header

            <header>
    <!-- Navbar -->
    <nav class="navbar mt-2 d-flex navbar-expand-lg navbar-light bg-white shadow-sm">
      <div class="container   justify-content-center">
        <a class="navbar-brand m-4  justify-content-center col-lg-4 col-md-6 col-sm-8 " href="#">
          <img
            src="https://raw.githubusercontent.com/Sektor30/dise-oProyecto3/56a43910486b5ee983d60923b601c07e96cf0481/assets/Group%201.png"
            alt="Logo"
            width="60%"
            class="logo d-flex m-auto" 
          />
        </a>

        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ms-auto  d-flex justify-content-center">

            <li class="nav-item m-auto"><a class="nav-link " href="./pages/red.html">Red</a></li>
            <li class="nav-item m-auto"><a class="nav-link" href="./pages/procesos.html">Procesos</a></li>
            <li class="nav-item m-auto"><a class="nav-link" href="./pages/publicaciones.html">Publicaciones</a></li>
            <li class="nav-item m-auto"><a class="nav-link" href="./pages/contacto.html">Contacto</a></li>
          </ul>
        </div>
      </div>
    </nav>
  </header>


  <div class="container  rounded col-lg-4" style="max-height: 300px; overflow: hidden;">
          <div class="row justify-content-center">
            <div class="col-lg-12 col-md-12">
              <div id="masoLogoCarousel" class="carousel slide" data-bs-ride="carousel">
                <div class="carousel-indicators">
                  <button type="button" data-bs-target="#masoLogoCarousel" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
                  <button type="button" data-bs-target="#masoLogoCarousel" data-bs-slide-to="1" aria-label="Slide 2"></button>
                  <button type="button" data-bs-target="#masoLogoCarousel" data-bs-slide-to="2" aria-label="Slide 3"></button>
                </div>
                
                <div class="carousel-inner">
                  <div class="carousel-item active">
                    <div class="logo-carousel-item">
                      <img src="https://github.com/satelite30/-logossitio/blob/main/logo03.png?raw=true"
                       alt="Logo Grupo MASO 1" class="logo-carousel-img " >
                      <div class="logo-carousel-caption">
                        <h3>Medio Ambiente y Sociedad</h3>
                        <p>Investigación y transformación social</p>
                      </div>
                    </div>
                  </div>
                  
                  <div class="carousel-item">
                    <div class="logo-carousel-item">
                      <img src="https://github.com/satelite30/-logossitio/blob/main/logo03.png?raw=true"
                       alt="Logo Grupo MASO 2" class="logo-carousel-img ">
                      <div class="logo-carousel-caption">
                        <h3>Universidad de Antioquia</h3>
                        <p>Facultad de Ciencias Sociales y Humanas</p>
                      </div>
                    </div>
                  </div>
                  
                  <div class="carousel-item">
                    <div class="logo-carousel-item">
                      <img src="https://github.com/satelite30/-logossitio/blob/main/logo03.png?raw=true"
                       alt="Logo Grupo MASO 3" class="logo-carousel-img ">
                      <div class="logo-carousel-caption">
                        <h3>Grupo MASO</h3>
                        <p>Planeación, Ciudadanía, Territorio y Ambiente</p>
                      </div>
                    </div>
                  </div>
                </div>
        
                <button class="carousel-control-prev" type="button" data-bs-target="#masoLogoCarousel" data-bs-slide="prev">
                  <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                  <span class="visually-hidden">Previous</span>
                </button>
                <button class="carousel-control-next" type="button" data-bs-target="#masoLogoCarousel" data-bs-slide="next">
                  <span class="carousel-control-next-icon" aria-hidden="true"></span>
                  <span class="visually-hidden">Next</span>
                  </button>
              </div>
            </div>
          </div>
          </div>



          ---------------------------modales  pdf activador 2018--------

      <div class="subtitulos text-center">
            <h3>Conoce  <span style="color: #004200;">más</span>   </h3>
          </div>

           <div class="row justify-content-center  my-5 gap-4  ">
            <div class="col-md-5 text-center mb-4 mb-md-0 ">
              <button type="button" class="pdf-btn" data-bs-toggle="modal" data-bs-target="#pdfModalMedellin">
                <i class="fa-solid fa-file-pdf text-danger "></i>
                <span class="pdf-label">Informe General de Investigación Medellín</span>
              </button>
            </div>
            <div class="col-md-5 text-center">
              <button type="button" class="pdf-btn" data-bs-toggle="modal" data-bs-target="#pdfModalRio">
                <i class="fa-solid fa-file-pdf text-danger"></i>
                <span class="pdf-label">Informe General de Investigación Río de Janeiro</span>
              </button>
            </div>
          </div>