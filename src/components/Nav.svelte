<script>
  export let segment;
</script>

<style>
  [aria-current] {
    position: relative;
    display: inline-block;
  }

  [aria-current]::after {
    position: absolute;
    content: "";
    width: calc(100% - 10px);
    height: 2px;
    background-color: rgb(58, 70, 107);
    display: block;
    bottom: 0;
    left: 5px;
  }

  a {
    text-decoration: none;
    padding: 1em 0.5em;
    display: block;
  }

  .menuContainer {
    display: block;
    align-items: center;
  }
  .menuFullWidth {
    border-bottom: solid 1px #f1f1f1;
    -webkit-box-shadow: 0 -30px 40px 0 rgba(0, 0, 0, 0.75);
    -moz-box-shadow: 0 -30px 40px 0 rgba(0, 0, 0, 0.75);
    box-shadow: 0 -30px 40px 0 rgba(0, 0, 0, 0.75);
    background-color: #fff;
    position: relative;
  }

  .logo {
    width: 100%;
    text-align: center;
  }

  .menu {
    width: 100%;
    text-align: center;
    padding: 10px;
  }

  .menu a {
    padding: 5px 10px;
    font-size: 14px;
    display: inline-block;
  }

  .logo img {
    max-width: 75px;
  }

  @media screen and (min-width: 900px) {
    .menuFullWidth {
      position: fixed;
      background-color: #fff;
      z-index: 5;
    }

    .logo {
      flex: 1;
      text-align: left;
    }

    .menu {
      width: auto;
      text-align: right;
      padding: 0;
    }

    .menu a {
      padding: 15px;
    }

    .menuContainer {
      display: flex;
      align-items: center;
    }

    .logo img {
      max-width: 100px;
    }
  }
</style>

<header id="" class="menuFullWidth flexContainer">
  <div class="flexContent">
    <div class="menuContainer" style="width:100%">
      <div class="logo">
        <img
          loading="lazy"
          src="/images/jos-de-berdt-logo.jpg"
          alt="Jos De Berdt" />
      </div>
      <nav class="menu">
        <a aria-current={segment === undefined ? 'page' : undefined} href=".">
          Home
        </a>
        <a aria-current={segment === 'about' ? 'page' : undefined} href="about">
          Who
        </a>
      </nav>
    </div>
  </div>
</header>
