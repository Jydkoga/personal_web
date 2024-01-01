<body>
  <div class="grid">
    <nav class="nav">
      <nav class="top-nav">
        <button class="logoBtn">
          <img
            alt="Koga Logo"
            src={"src/lib/assets/kogaLogo.png"}
            width="30"
            height="30"
          />
          Home
        </button>
        <div>Search</div>
      </nav>
      <nav class="bottom-nav">bottom nav</nav>
    </nav>
    <div class="main-body">Column2</div>
  </div>
</body>
<footer>
  <div class="footer">footer</div>
</footer>

<style>
  .grid {
    display: grid;
    padding: 0%;
    grid-template-columns: minmax(150px, 20%) 80%;
    min-height: 100vh;
  }
  body {
    margin: 5px;
    padding: 0;
    background-color: #000000;
    font-family: "Yantramanav", sans-serif;
    color: white;
  }
  .nav {
    background-color: #000000;
    min-height: 100%;
    display: grid;
    grid-template-rows: minmax(50px, 15%) 85%;
  }
  .top-nav {
    background-color: #181818;
    border-radius: 15px;
    padding: 20px;
    width: 240px;
    height: 60px;
    grid-template-rows: 1fr 1fr;
  }
  .bottom-nav {
    background-color: #181818;
    border-radius: 15px;
    padding: 20px;
    width: 240px;
    height: 100%;
  }
  .main-body {
    background-image: linear-gradient(180deg, rgb(48, 48, 83), #181818);
    min-height: 100%;
    border-radius: 15px;
    padding: 20px;
    width: 100%;
  }
  .footer {
    position: fixed;
    left: 0;
    bottom: 0;
    height: 75px;
    width: 100%;
    background-color: black;
    text-align: center;
  }
  .logoBtn {
    background-color: transparent;
    border: none;
    color: white;
    font-family: "Yantramanav", sans-serif;
  }
  .logoBtn:hover {
    cursor: pointer;
  }
</style>
