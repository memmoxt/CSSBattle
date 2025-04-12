<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
	    margin: 0;
	    padding: 0;
	    box-sizing: content-box;
	    --yellow: #f3ac3c;
	    --green: #1a4341;
	}

	.main {
	    height: 300px;
	    width: 400px;
	    display: flex;
	    justify-content: center;
	    align-items: center;
	    position: absolute;
	    overflow: hidden;
        background-color: var(--yellow);

	    &>div:nth-child(1),
	    &>div:nth-child(2) {
	        position: absolute;
	        height: 101px;
	        aspect-ratio: 1;
	        background-color: var(--green);
	        border-radius: 10px;
	        transform: translate(-85px, -35px);
	        /* opacity: 0.5; */

	        &:before {
	            position: absolute;
	            content: '';
	            height: 51px;
	            width: 100px;
	            border-radius: 10px;
	            transform: translate(51px, 0px);
	            background-color: var(--green);
	        }

	        &:after {
	            position: absolute;
	            content: '';
	            height: 20px;
	            width: 20px;
	            background-color: var(--green);
	            transform: translate(95px, 44px);
	        }
	    }

	    &>div:nth-child(2) {
	        transform: scale(-1) translate(-86px, -36px);
	    }

        &>div:nth-child(3){
            position:absolute;
            height:70px;
            aspect-ratio:1;
            background-color:var(--yellow);
            border-radius:10px;
        }
	}
</style>
