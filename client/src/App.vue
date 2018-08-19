<template>
  <div id="app">

    <h1 id="title">Niedźwiedź</h1>
    <h3>Welcome to the official <strong>Niedźwiedź</strong> website.</h3>


    <p>Links you might be interested in:</p>
    <ul id="useful-links">
      <li>
        <a href="https://www.youtube.com/channel/UCPrQ6QT_-k0YpgJclL1ks4w">
          YouTube <i class="fab fa-youtube"></i>
        </a>
      </li>
      <li>
        <a href="https://www.facebook.com/niedzwiedzw/">
          Facebook <i class="fab fa-facebook-square"></i>
        </a>
      </li>
      <li>
        <a href="https://www.instagram.com/niedzwiedzwo/">
           Instagram <i class="fab fa-instagram"></i>
        </a>
      </li>
      <li>
        <a href="https://open.spotify.com/artist/47DkO7js1AuBmqmRXCFA6l?si=2TLFj3EuTJiXR7gAguRP5g">
          Spotify <i class="fab fa-spotify"></i>
        </a>
      </li>
    </ul>


    <div id="media-container">

      <!--SPOTIFY-->
      <iframe src="https://open.spotify.com/embed/artist/47DkO7js1AuBmqmRXCFA6l"
              width="100%"
              height="280"
              frameborder="0"
              allowtransparency="true"
              allow="encrypted-media">
      </iframe>

      <br>
      <!--FACEBOOK-->
      <iframe src="https://www.facebook.com/plugins/video.php?href=https%3A%2F%2Fwww.facebook.com%2Fniedzwiedzw%2Fvideos%2F2107141302945899%2F&show_text=1&width=476"
              width="100%"
              height="488"
              style="border:none;overflow:hidden"
              scrolling="no"
              frameborder="0"
              allowTransparency="true"
              allow="encrypted-media"
              allowFullScreen="true">
      </iframe>

    </div>
  </div>
</template>

<script>
  export default {
    name: 'App'
  }
</script>

<style lang="scss">
  #media-container{
    max-width: 480px;
    margin-left: auto;
    margin-right: auto;
    & > *:hover {
      transform: translate3d(2px, -2px, 0);
    }
  }
  li {
    list-style-type: none;
  }
  body {
    background-size: cover;
    background-image: url("../static/background.png");
    margin-bottom: 15rem;
  }
  * {
    transition: all 0.3s;
  }

  #useful-links{
    margin: 2rem;
    line-height: 2rem;
    li {
      a {
        font-size: 1.7rem;
      }
    }
  }

  a {
    text-decoration: none;
    color: #ffbd72;
    &:hover {
      opacity: 0.6;
    }
  }

  h1 {
    color: #1f32ad;
    &:hover{
      color: inherit;
    }
  }

  strong {
    &:hover {
      color: #1f32ad;
    }
  }
  #app {
    font-family: 'Poppins', 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: lightgray;
    margin-top: 60px;
  }

  #title {
    font-size: 5rem;
  }

  @media only screen and (max-width: 600px) {
    #title {
      font-size: 3rem;
    }
  }
</style>
