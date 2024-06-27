<div class="main">
  <div class="center"></div>
  <div class="square"></div>
</div>

<style>
  * {
    margin: 0;
    padding: 0;
  }

  .main {
    height: 300px;
    width: 400px;
    display: flex;
    justify-content: center;
    align-items: center;

    .square {
      position: absolute;
      height: 50px;
      width: 50px;
      transform: rotate(45deg);
      background-color: #FBE18C;
      z-index: 0;
    }

    .center {
      position: absolute;
      transform: rotate(45deg);
      height: 50px;
      width: 50px;


      &:before {
        content: '';
        position: absolute;
        height: 200px;
        width: 50px;
        background-color: #A3A368;
        z-index: -1;
        transform: translate(0px, -75px);
      }

      &:after {
        content: '';
        position: absolute;
        width: 200px;
        height: 50px;
        background-color: #F3AC3C;
        z-index: -1;
        transform: translate(-75px, 0px);
      }
    }

  }
</style>
