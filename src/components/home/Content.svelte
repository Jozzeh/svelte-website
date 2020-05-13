<style>
  #homePerson {
    display: block;
    border-top: solid 1px var(--light-grey-color);
    border-bottom: solid 1px var(--light-grey-color);
    padding: 15px 0 25px 0;
  }

  #homePersonLeft {
    font-size: 80px;
    width: 100%;
    color: var(--dark-grey-color);
    line-height: 1;
  }

  #homeIntroHeading {
    font-size: 24px;
    padding: 25px 0;
    color: var(--darker-grey-color);
  }

  #homeIntro {
    display: flex;
    flex-wrap: wrap;
    align-items: flex-end;
  }

  .homeIntroContent {
    width: 100%;
    border: solid 1px var(--darker-grey-color);
    margin-bottom: 15px;
  }

  .homeIntroTitle {
    background-color: var(--darker-grey-color);
    color: #fff;
    font-size: 18px;
    padding: 15px 25px;
  }

  .homeIntroList {
    line-height: 36px;
    font-size: 16px;
    padding: 15px 25px;
  }

  #homeIntroMid .homeIntroTitle {
    background-color: var(--light-grey-color);
    color: var(--darker-grey-color);
  }

  #homeIntroMid .homeIntroList {
    background-color: var(--darker-grey-color);
    color: #fff;
  }

  #homePersonRight h1,
  #homePersonRight h2 {
    font-size: 28px;
    font-weight: 400;
    color: #000;
  }

  @media screen and (min-width: 900px) {
    #homePerson {
      display: flex;
      border-top: solid 2px var(--light-grey-color);
      border-bottom: solid 2px var(--light-grey-color);
      padding: 25px 0;
      margin: 25px 15px;
    }

    #homePersonLeft {
      font-size: 320px;
      width: 50%;
      color: var(--dark-grey-color);
    }

    #homePersonRight {
      flex: 1;
      display: flex;
      flex-direction: column;
      justify-content: flex-end;
    }
    #homePersonRight p {
      margin-top: 25px;
      line-height: 32px;
    }

    #homePersonSmall {
      width: 100%;
      font-size: 24px;
    }

    #homeIntroHeading {
      font-size: 32px;
      text-align: center;
    }

    .homeIntroContent {
      width: calc(33% - 10px);
      margin: 0 5px;
    }

    #homePersonRight h1,
    #homePersonRight h2 {
      width: 100%;
      font-size: 60px;
      font-weight: 400;
      color: #000;
    }

    #homePersonRight h2 {
      font-size: 40px;
    }
  }
</style>

<div id="content" class="flexContainer">
  <div class="flexContent">
    <div id="homePerson">
      <div id="homePersonLeft">Hi,</div>
      <div id="homePersonRight">
        <p id="homePersonSmall">my name is...</p>
        <h1>Jos De Berdt</h1>
        <p>and I'm a</p>
        <h2>front-end developer</h2>
      </div>
    </div>
    <h2 id="homeIntroHeading">Where do I use JavaScript?</h2>
    <div id="homeIntro">
      <div class="homeIntroContent panel" id="homeIntroLeft">
        <div class="homeIntroTitle">Server</div>
        <div class="homeIntroList">
          <ul>
            <li>NodeJs</li>
            <li>Express</li>
            <li>Adonis</li>
            <li>PM2</li>
            <li>RTC / Sockets</li>
          </ul>
        </div>
      </div>
      <div class="homeIntroContent panel" id="homeIntroMid">
        <div class="homeIntroTitle">Browser</div>
        <div class="homeIntroList">
          <ul>
            <li>Native JavaScript</li>
            <li>EcmaScript (ES6)</li>
            <li>React</li>
            <li>Svelte</li>
            <li>Redux</li>
            <li>Micro front-ends</li>
            <li>Service Workers</li>
          </ul>
        </div>
      </div>
      <div class="homeIntroContent panel" id="homeIntroRight">
        <div class="homeIntroTitle">Desktop / Mobile</div>
        <div class="homeIntroList">
          <ul>
            <li>React Native</li>
            <li>Electron</li>
            <li>Node-Red</li>
            <li>CLI tools</li>
            <li>Proton native</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</div>
