<div class="main">
  <div class="first">
    <div class="inside"></div>
  </div>
  <div class="bigger-circle">
    <div class="grid">
      <div></div>
      <div></div>
      <div></div>
    </div>
  </div>
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
    background: #1A4341;

    .first {
      height: 200px;
      aspect-ratio: 1;
      border-radius: 50%;
      background-color: #998235;
      position: relative;
      overflow: hidden;

      &>.inside {
        content: '';
        position: absolute;
        height: 140px;
        width: 200px;
        background-color: #1A4341;
        transform: translate(0, 30px);
      }
    }

    .bigger-circle {
      position: absolute;
      border-radius: 50%;
      height: 250px;
      aspect-ratio: 1;
      overflow: hidden;

      .grid {
        position: absolute;
        display: grid;
        height: 140px;
        width: 140px;
        transform: translate(-75px, 55.0px);
        grid-template-rows: repeat(3, 20px);
        padding: 20px 0;
        gap: 20px;

        &>div {
          height: 20px;
          width: 400px;
          background-color: #F3AC3C;
        }
      }
    }
  }
</style>
