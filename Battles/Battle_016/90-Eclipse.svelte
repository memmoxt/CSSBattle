<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
	    margin: 0;
	    padding: 0;
	    box-sizing: content-box;
	    --amber: #998235;
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
        background-color:var(--yellow);

	    &>div:nth-child(1) {
	        position: absolute;
	        height: 400px;
	        aspect-ratio: 1;
	        background-color: var(--amber);
	        /* opacity: 0.5; */
	        border-radius: 50%;
	        transform: translate(0, -200px);
	    }

	    &>div:nth-child(2) {
            z-index: 2;
	        height: 200px;
	        aspect-ratio: 1;
	        background-color: var(--green);
	        /* opacity: 0.5; */
	        border-radius: 50%;
	        box-shadow: 0 0 0 25px var(--yellow);

	        &:before {
	            content: '';
	            position: absolute;
	            height: 400px;
	            aspect-ratio: 1;
	            background-color: var(--amber);
	            transform: translate(-100px, 100px);
	            border-radius: 50%;
	        }
	    }

	}
</style>

