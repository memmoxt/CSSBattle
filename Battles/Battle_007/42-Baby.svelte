<div class="main">
  <div class="head">
    <div class="hair"></div>
    <div class="hair"></div>
    <div class="eye"></div>
    <div class="eye"></div>
    <div class="mouth"></div>
  </div>
</div>
<style>
  * {
    margin: 0;
    padding: 0;
    background: #293462;
  }

  .main {
    height: 300px;
    width: 400px;
    display: flex;
    justify-content: center;
    align-items: center;

    .head {
      height: 200px;
      aspect-ratio: 1;
      border-top-right-radius: 50%;
      border-top-left-radius: 50%;
      border-bottom-left-radius: 25%;
      border-bottom-right-radius: 25%;
      background-color: #FE5F55;
      overflow: hidden;

      display: flex;
      justify-content: center;
      align-items: center;
      flex-wrap: wrap;
      align-content: center;

      &>.hair {
        height: 100px;
        aspect-ratio: 1;
        border-radius: 50%;
        transform: translate(0, -65px);
        background-color: #FFF1C1;
      }

      &>.eye {
        height: 60px;
        aspect-ratio: 1;
        border-radius: 50%;
        margin: 0 20px;
        transform: translate(0, -25px);
        background-color: #FFF1C1;
      }

      &>.mouth {
        height: 10px;
        width: 40px;
        border-radius: 5px;
        background-color: #FFF1C1;
        transform: translate(0, -5px);
      }
    }
  }
</style>
