<div class="main">
  <div class="rectangle">
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
  </div>
</div>
<style>
  * {
    margin: 0;
    padding: 0;
    background: #1A4341;
  }

  .main {
    height: 300px;
    width: 400px;
    display: flex;
    justify-content: center;
    align-items: center;

    &>.rectangle {
      height: 120px;
      width: 260px;
      display: grid;
      gap: 20px;
      grid-template-columns: repeat(4, 50px);
      grid-template-rows: repeat(2, 50px);

      &>div {

        height: 50px;
        background-color: #998235;
        border-radius: 50%;
        aspect-ratio: 1;
      }

      &>div:nth-child(2),
      div:nth-child(3) {
        border-bottom-left-radius: 0%;
        border-bottom-right-radius: 0%;
      }

      &>div:nth-child(5),
      div:nth-child(8) {
        border-top-left-radius: 0%;
        border-top-right-radius: 0%;
      }

      &>div:nth-child(2),
      div:nth-child(4),
      div:nth-child(5),
      div:nth-child(7) {
        background-color: #F3AC3C;
      }

    }
  }
</style>
