<div class="main">
  <div class="star-box"></div>
</div>

<style>
  * {
    margin: 0;
    padding: 0;
    background: #f3ac3c;
  }

  .main {
    height: 300px;
    width: 400px;
    display: flex;
    justify-content: center;
    align-items: center;

    .star-box {
      height: 200px;
      aspect-ratio: 1;
      background-color: #1a4341;
      overflow: hidden;

      &:before {
        content: '';
        position: absolute;
        height: 200px;
        aspect-ratio: 1;
        border-radius: 50%;
        transform: translate(50%, 50%);
        background-color: #f3ac3c;
        box-shadow:
          -200px 0px #f3ac3c,
          0px -200px #f3ac3c,
          -200px -200px #f3ac3c;
      }
    }
  }
</style>
