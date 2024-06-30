<div class="main">
	<div class="orange-control">
		<div class="orange"></div>
	</div>
	<div class="blue-control">
		<div class="blue"></div>
	</div>
</div>
<style>
	* {
	  margin: 0;
	  padding: 0;
	}

	.main {
	  width: 100vw;
	  height: 100vh;
	  background: #222;
	  display: flex;
	  justify-content: center;
	  align-items: center;

	  .orange-control {
	    transform: translate(23.0px, -27.0px);
	  }

	  .orange {
	    width: 44px;
	    height: 70px;
	    background-color: transparent;
	    border-top: 0px solid transparent;
	    border-right: 0px solid transparent;
	    border-left: 30px solid #F2994A;
	    border-bottom: 30px solid #F2994A;
	    border-bottom-left-radius: 13%;
	    transform: rotate(45deg);

	    &:after {
	      content: "";
	      position: absolute;
	      height: 30px;
	      width: 30px;
	      background-color: #F2994A;
	      border-top-right-radius: 20.0%;
	      transform: translate(69.0%, 233%);
	    }
	  }

	  .blue-control {
	    transform: translate(-24.09px, 26px);
	  }

	  .blue {
	    width: 44px;
	    height: 70px;
	    background-color: transparent;
	    border-top: 0px solid transparent;
	    border-right: 0px solid transparent;
	    border-left: 30px solid #2D9CDB;
	    border-bottom: 30px solid #2D9CDB;
	    border-bottom-left-radius: 13%;
	    transform: rotate(-135deg);

	    &:after {
	      content: "";
	      position: absolute;
	      height: 30px;
	      width: 30px;
	      background-color: #2D9CDB;
	      border-top-right-radius: 20.0%;
	      transform: translate(69.0%, 233%);
	    }
	  }
	}
	}
</style>
