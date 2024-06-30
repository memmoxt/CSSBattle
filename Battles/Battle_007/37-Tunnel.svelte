<div class="main">
  <div></div>
  <div></div>
  <div></div>
</div>
<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    background: #6592CF;
  }

  .main {
    height: 300px;
    width: 400px;
    display: flex;
    justify-content: center;
    align-items: center;

    &>div:nth-child(1) {
      height: 250px;
      aspect-ratio: 1;
      background-color: #243D83;
    }

    &>div:nth-child(2) {
      position: absolute;
      height: 150px;
      aspect-ratio: 1;
      transform: rotate(15deg);
      background-color: #6592CF;
    }

    &>div:nth-child(3) {
      position: absolute;
      height: 75px;
      aspect-ratio: 1;
      transform: rotate(30deg);
      background-color: #243D83;
    }
  }
</style>
