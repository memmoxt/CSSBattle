<div class="main">
  <div class="vanilla"></div>
</div>


<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    background: #293462;
  }

  .main {
    height: 300px;
    width: 400px;
    display: flex;
    justify-content: center;
    align-items: center;

    .vanilla {
      height: 100px;
      width: 100px;
      background-color: #FFF1C1;
      border-bottom-right-radius: 20px;
      border-bottom-left-radius: 20px;

      &:before {
        content: '';
        position: absolute;
        height: 100px;
        aspect-ratio: 1;
        transform: translate(0, -50%);
        border-top-right-radius: 50px;
        border-top-left-radius: 50px;
        background-color: #fff1c1;
      }

      &:after {
        content: '';
        position: absolute;
        height: 40px;
        width: 30px;
        background-color: #FE5F55;
        transform: translate(35px, 110px);
        border-bottom-right-radius: 10px;
        border-bottom-left-radius: 10px;
        box-shadow: 0px -10px 0px #A64942;
      }
    }
  }
</style>
