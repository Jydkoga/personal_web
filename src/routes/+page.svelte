<body>
  <div class="main-container">
    <nav class="nav">
      <nav class="top-nav">
        <button class="button logo">
          <img
            alt="Koga Logo"
            src={"src/lib/assets/kogaLogo.png"}
            width="25"
            height="25"
          />
          <div class="button-text">Home</div>
        </button>
        <button class="button search">
          <img
            alt="Search Icon"
            src={"src/lib/assets/search.png"}
            width="25"
            height="25"
            style="filter: brightness(0) invert(1)"
          />
          <div class="button-text">Search</div>
        </button>
      </nav>
      <nav class="bottom-nav">
        <div class="library-container">
          <button class="button library">
            <img
              alt="library-icon"
              src={"src/lib/assets/library.png"}
              width="25"
              height="25"
              style="filter: brightness(0) invert(1)"
            />
            <div class="button-text">James's Library</div>
          </button>
        </div>
        <div class="social-conveyor-container">
          <div class="social-conveyor">
            <div class="social-container">
              <button class="social-button">
                <img
                  alt="Instagram-icon"
                  src={"src/lib/assets/instagram.png"}
                  width="25"
                  height="25"
                />
              </button>
              <div class="social-text">Instagram</div>
            </div>
            <div class="social-container">
              <button class="social-button">
                <img
                  alt="LinkedIn-icon"
                  src={"src/lib/assets/linkedin.png"}
                  width="25"
                  height="25"
                />
              </button>
              <div class="social-text">LinkedIn</div>
            </div>
            <div class="social-container">
              <button class="social-button">
                <img
                  alt="Spotify-icon"
                  src={"src/lib/assets/spotify.png"}
                  width="25"
                  height="25"
                />
              </button>
              <div class="social-text">Spotify</div>
            </div>
            <div class="social-container">
              <button class="social-button">
                <img
                  alt="Github-icon"
                  src={"src/lib/assets/github.png"}
                  width="25"
                  height="25"
                />
              </button>
              <div class="social-text">Github</div>
            </div>
          </div>
          <button class="button">
            <div class="social-arrow">
              <img
                alt="arrow-icon"
                src={"src/lib/assets/right_arrow.png"}
                width="25"
                height="25"
                style="filter: brightness(0) invert(1)"
              />
            </div>
          </button>
          <div class="mask"></div>
        </div>
        <div class="albums">
          <button class="album-button">
            <img
              class="album-image"
              alt="Album Cover"
              src={"src/lib/assets/madvillainy.png"}
            />
            <div class="album-info">
              <div class="album-text">About</div>
              <div class="made-by">Playlist &#183; James Koga</div>
            </div>
          </button>
          <button class="album-button">
            <img
              class="album-image"
              alt="Album Cover"
              src={"src/lib/assets/madvillainy.png"}
            />
            <div class="album-info">
              <div class="album-text">Projects</div>
              <div class="made-by">Playlist &#183; James Koga</div>
            </div>
          </button>
          <button class="album-button">
            <img
              class="album-image"
              alt="Album Cover"
              src={"src/lib/assets/madvillainy.png"}
            />
            <div class="album-info">
              <div class="album-text">Music</div>
              <div class="made-by">Playlist &#183; James Koga</div>
            </div>
          </button>
          <button class="album-button">
            <img
              class="album-image"
              alt="Album Cover"
              src={"src/lib/assets/madvillainy.png"}
            />
            <div class="album-info">
              <div class="album-text">Contact</div>
              <div class="made-by">Playlist &#183; James Koga</div>
            </div>
          </button>
        </div>
      </nav>
    </nav>
    <div class="main-body">Column2</div>
  </div>
</body>
<footer>footer</footer>

<style>
  .main-container {
    display: flex;
    padding: 0%;
    height: calc(100vh - 90px);
    margin-right: 0%;
    /* background-color: red; */
    /* min-height: 100vh; */
  }
  body {
    margin: 5px;
    padding: 0;
    background-color: black;
    font-family: "Yantramanav", sans-serif;
    color: white;
    font-size: large;
    max-height: calc(100vh - 90px);
    overflow-y: auto;
  }
  .nav {
    flex: 25%;
    margin-right: 8px;
    background-color: #000000;
    min-height: 100%;
    display: flex;
    flex-direction: column;
  }
  .top-nav {
    flex: 12%;
    background-color: #121212;
    border-radius: 15px;
    padding: 20px;
    width: 240px;
    display: flex;
    flex-direction: column;
  }
  .button {
    background-color: transparent;
    border: none;
    display: flex;
  }
  .button.logo {
    padding-top: 0%;
  }
  .button.search {
    margin-top: 10px;
  }
  .button img {
    padding-right: 20px;
  }
  .button:hover {
    cursor: pointer;
  }
  .button-text {
    color: white;
    font-family: "Yantramanav", sans-serif;
    font-size: large;
    font-weight: bold;
    /* padding-top: 3px; */
    display: inline-block;
    position: relative;
  }
  /* got hover from: https://www.30secondsofcode.org/css/s/hover-underline-animation/ */
  .button-text::after {
    content: "";
    position: absolute;
    width: 100%;
    transform: scaleX(0);
    height: 2px;
    bottom: 0;
    left: 0;
    background-color: #65d36e;
    transform-origin: bottom right;
    transition: transform 0.25s ease-out;
  }
  .button-text:hover::after {
    transform: scaleX(1);
    transform-origin: bottom left;
  }
  .bottom-nav {
    flex: 88%;
    margin-top: 10px;
    background-color: #121212;
    border-radius: 15px;
    padding: 20px;
    width: 240px;
    height: 100%;
    display: flex;
    flex-direction: column;
  }
  .bottom-nav .library-container {
    margin-bottom: 10px;
  }

  .button.library img {
    margin-right: -10px;
  }
  .social-conveyor-container {
    position: relative;
    z-index: 1;
    overflow: hidden;
    display: flex;
    margin-bottom: 10px;
  }
  .social-conveyor-container button {
    background-color: red;
  }
  .social-arrow {
    border-radius: 15px;
    height: 6px;
    width: 6px;
    padding: 10px;
    background-color: #242424;
    position: absolute;
    right: 0;
    z-index: 3;
    display: flex;
    justify-content: center;
  }
  .social-arrow img {
    display: block;
    scale: 70%;
    margin: -9px 0 0 17px;
    opacity: 90%;
  }
  .mask {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: linear-gradient(
      to left,
      rgba(18, 18, 18, 1),
      rgba(18, 18, 18, 0)
    );
    z-index: 2;
  }
  .social-conveyor {
    display: flex;
    margin-left: 0;
    /* position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: black;
    opacity: 0.5;
    z-index: 2; */
  }
  .social-conveyor .social-container {
    /* z-index: 1;
    position: relative; */
    display: flex;
    padding-top: 2px;
    padding-bottom: 2px;
    padding-right: 7px;
    border-radius: 15px;
    background-color: #242424;
    margin-right: 7px;
  }
  .social-conveyor .social-button {
    height: 25px;
    width: 25px;
    border-radius: 50%;
    text-align: center;
    border: none;
    background-color: rgb(223, 14, 14);
    margin-right: 5px;
  }
  .social-button img {
    display: block;
    scale: 75%;
    margin: -1px 0 0 -4px;
  }
  .social-button:hover {
    cursor: pointer;
  }
  .social-conveyor .social-text {
    margin-top: 2px;
    color: white;
    font-family: "Yantramanav", sans-serif;
    font-size: medium;
  }
  .bottom-nav .albums {
    flex: 90%;
    /* background-color: blue; */
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
  }
  .main-body {
    background-image: linear-gradient(180deg, rgb(48, 48, 83), #181818);
    min-height: 100%;
    border-radius: 15px;
    padding: 20px;
    width: 100%;
  }

  .album-button {
    border: none;
    background-color: transparent;
    display: flex;
    justify-content: row;
    margin-bottom: 10px;
    border-radius: 8px;
  }

  .album-button:hover {
    background-color: #1a1a1a;
    cursor: pointer;
  }

  .album-info {
    display: flex;
    flex-direction: column;
    margin-top: 8px;
    margin-left: 3px;
  }
  .album-text {
    color: white;
    font-family: "Yantramanav", sans-serif;
    font-size: large;
    font-weight: bold;
    text-align: left;
  }
  .album-image {
    /* background-color: red; */
    border-radius: 8px;
    margin-left: 0;
    margin-right: 5px;
    margin-top: 5px;
    width: 50px;
    height: 50px;
  }
  .made-by {
    color: lightgray;
  }
  footer {
    height: 90px;
    text-align: center;
    background-color: black;
    display: flex;
    align-items: center;
    justify-content: center;

    /* position: fixed; */
    /* left: 0;
    bottom: 0; */
    /* width: 100%; */
  }
</style>
