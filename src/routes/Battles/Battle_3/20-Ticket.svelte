<div class="main">
	<div class="yellow-box"></div>
	<div class="amber-box"></div>
	<span class="ball"></span>
	<span class="ball-1"></span>
</div>
<style>
	* {
	  margin: 0;
	  padding: 0;
	  background: #62306D;
	}

	.main {
	  height: 100vh;
	  width: 100vw;
	  display: flex;
	  justify-content: center;
	  align-items: center;

	  .ball {
	    position: absolute;
	    height: 20px;
	    aspect-ratio: 1;
	    border-radius: 50%;
	    transform: translate(40px, 50px);
	    background-color: #62306D;
	  }

	  .ball-1 {
	    position: absolute;
	    height: 20px;
	    aspect-ratio: 1;
	    border-radius: 50%;
	    transform: translate(40px, -50px);
	    background-color: #62306D;
	  }

	  &>.yellow-box {
	    height: 100px;
	    width: 140px;
	    background-color: #F7EC7D;

	    &:before {
	      content: "";
	      position: absolute;
	      height: 39px;
	      aspect-ratio: 1;
	      border-radius: 50%;
	      background-color: #62306D;
	      transform: translate(-50%, -50%);
	    }

	    &:after {
	      content: "";
	      position: absolute;
	      height: 39px;
	      aspect-ratio: 1;
	      border-radius: 50%;
	      background-color: #62306D;
	      transform: translate(-50%, 205%);
	    }

	  }

	  &>.amber-box {
	    height: 100px;
	    width: 60px;
	    background-color: #e38f66;

	    &:before {
	      content: "";
	      position: absolute;
	      height: 39px;
	      aspect-ratio: 1;
	      border-radius: 50%;
	      background-color: #62306D;
	      transform: translate(102%, -50%);
	    }

	    &:after {
	      content: "";
	      position: absolute;
	      height: 39px;
	      aspect-ratio: 1;
	      border-radius: 50%;
	      background-color: #62306D;
	      transform: translate(102%, 205%);
	    }
	  }
	}

	}
</style>
