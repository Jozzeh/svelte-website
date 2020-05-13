<style>
  #heroContainer {
    height: 75vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: var(--light-grey-color);
  }

  .heroText {
    line-height: 22px;
    padding: 15px 0;
    color: var(--dark-grey-color);
    text-align: center;
  }

  .heroSmaller {
    font-size: 8px;
  }

  .heroContent {
    line-height: normal;
    position: relative;
    background-color: var(--light-grey-color);
    font-size: calc(100vw / 4);
    font-weight: 400;
    color: var(--light-grey-color);
    text-shadow: -1px 0 #000, 0 1px #000, 1px 0 #000, 0 -1px #000;
  }

  #heroLeft,
  #heroRight {
    z-index: 2;
  }
  #heroMid {
    position: absolute;
    z-index: 1;
  }

  @media screen and (min-width: 900px) {
    #heroContainer {
      height: 85vh;
    }

    .heroText {
      line-height: 36px;
      font-size: 20px;
    }

    .heroSmaller {
      font-size: 14px;
    }

    .heroContent {
      padding-top: 4vh;
    }
  }
</style>

<div id="heroContainer">
  <div class="heroContent" id="heroLeft">J</div>
  <div class="heroContent" id="heroMid">o</div>
  <div class="heroContent" id="heroRight">S</div>
</div>

<div class="heroText">
  I kinda like JavaScript.
  <br />
  <span class="heroSmaller">
    (and I hope the name never changes, because my intro just would not make any
    sense)
  </span>
</div>
