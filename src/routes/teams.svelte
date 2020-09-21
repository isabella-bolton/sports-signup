<style>
  /* ####### LAYOUT ####### */

  #grid-container {
    background-color: #1e387c;
    display: grid;
    grid-gap: 50px;
    grid:
      " nav     header  header  header  header  header  . " auto
      " y7-8    y10     y11     y12     y13     mix     . " auto
      " section notices notices notices notices .       . " auto
      " .       .       .       .       .       .       . " 60px
      / 1fr 1fr 1fr 1fr 1fr 1fr 1fr;
  }

  header {
    grid-area: header;
  }
  nav {
    grid-area: nav;
  }
  #y7-8 {
    grid-area: y7-8;
  }
  #y10 {
    grid-area: y10;
  }
  #y11 {
    grid-area: y11;
  }
  #y12 {
    grid-area: y12;
  }
  #y13 {
    grid-area: y13;
  }
  #mix {
    grid-area: mix;
  }
  section {
    grid-area: section;
  }
  #notices {
    grid-area: notices;
  }

  /* ####### STYLE ####### */
  nav {
    padding-left: 10px;
    padding-top: 10px;
  }

  header {
    padding-right: 300px;
  }

  #y7-8 {
    background-color: rgb(240, 230, 230);
    border-color: #ffc600;
    border-radius: 5%;
    padding-left: 10px;
    padding-right: 10px;
    padding-bottom: 10px;
  }
  #y10 {
    background-color: rgb(240, 230, 230);
    border-radius: 5%;
    padding-left: 10px;
    padding-right: 10px;
    padding-bottom: 10px;
  }
  #y11 {
    background-color: rgb(240, 230, 230);
    border-radius: 5%;
    padding-left: 10px;
    padding-right: 10px;
    padding-bottom: 10px;
  }
  #y12 {
    background-color: rgb(240, 230, 230);
    border-radius: 5%;
    padding-left: 10px;
    padding-right: 10px;
    padding-bottom: 10px;
  }
  #y13 {
    background-color: rgb(240, 230, 230);
    border-radius: 5%;
    padding-left: 10px;
    padding-right: 10px;
    padding-bottom: 10px;
  }
  #mix {
    background-color: rgb(240, 230, 230);
    border-radius: 5%;
    padding-left: 10px;
    padding-right: 10px;
    padding-bottom: 10px;
  }
  #notices {
    background-color: rgb(240, 230, 230);
    border-radius: 5px;
    padding-right: 10px;
  }
</style>

<div id="grid-container">
  <header>
    <h1 class="title is-1 title has-text-centered has-text-warning">Teams</h1>
  </header>

  <nav>
    <a class="button" href="/">Home</a>
  </nav>

  <div id="y7-8">
    <h1
      class="is-size-4 has-text-centered has-text-link has-text-weight-semibold">
      7&8
    </h1>
    <a class="button" href="teams/rangi-Y7-8">Rangi Year Y7&8</a>
  </div>

  <div id="y10">
    <h1
      class="is-size-4 has-text-centered has-text-link has-text-weight-semibold">
      10
    </h1>
    <a class="button" href="teams/rangi-intermediate-green">
      Rangi Intermediate Green
    </a>
    <a class="button" href="teams/rangi-intermediate-gold">
      Rangi Intermediate Gold
    </a>
    <a class="button" href="teams/rangi-intermediate-maroon">
      Rangi Intermediate Maroon
    </a>
  </div>

  <div id="y11">
    <h1
      class="is-size-4 has-text-centered has-text-link has-text-weight-semibold">
      11
    </h1>
    <a class="button" href="teams/rangi-intermediate-black">
      Rangi Intermediate Black
    </a>
    <a class="button" href="teams/rangi-intermediate-blue">
      Rangi Intermediate Blue
    </a>
    <a class="button" href="teams/rangi-intermediate-brown">
      Rangi Intermediate Brown
    </a>
    <a class="button" href="teams/rangi-intermediate-red">Intermediate Red</a>
  </div>

  <div id="y12">
    <h1
      class="is-size-4 has-text-centered has-text-link has-text-weight-semibold">
      12
    </h1>
    <a class="button" href="teams/rangi-open-maroon">Rangi Open Maroon</a>
    <a class="button" href="teams/rangi-open-gold">Rangi Open Gold</a>
    <a class="button" href="teams/rangi-open-green">Rangi Open Green</a>
  </div>

  <div id="y13">
    <h1
      class="is-size-4 has-text-centered has-text-link has-text-weight-semibold">
      13
    </h1>
    <a class="button" href="teams/rangi-open-blue">Rangi Open Blue</a>
    <a class="button" href="teams/rangi-open-yellow">Rangi Open Yellow</a>
  </div>

  <div id="mix">
    <h1
      class="is-size-4 has-text-centered has-text-link has-text-weight-semibold">
      Mix
    </h1>
    <a class="button" href="teams/rangi-senior-A">Rangi Senior A</a>
    <a class="button" href="teams/rangi-intermediate-A">Rangi Intermediate A</a>
    <a class="button" href="teams/rangi-intermediate-B">Rangi Intermediate B</a>
    <a class="button" href="teams/rangi-intermediate-yellow">
      Rangi Intermediate Yellow
    </a>
    <a class="button" href="teams/rangi-open-red">Rangi Open Red</a>
  </div>

  <section>
    <img src="/Basketball.png" alt="Basketballer" />
  </section>

  <div id="notices">
    <h2>
      <u>Notices:</u>
    </h2>
    <p>Don't forget your mouthguard.</p>
    <p>No game next friday, easter holiday</p>
  </div>
</div>
