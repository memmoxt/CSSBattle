<div class="main">
	<div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
	    margin: 0;
	    padding: 0;
	    box-sizing: content-box;
	    --blue: #4f77ff;
	    --black: #191919;
	    --yellow: #f9e492;
	    --shadowYellow: #d6b73f;
        background-color: var(--blue);
	}

	.main {
	    height: 300px;
	    width: 400px;
	    display: flex;
	    justify-content: center;
	    align-items: center;
	    position: absolute;
	    overflow: hidden;

	    &>div:nth-child(1) {
	        height: 200px;
	        aspect-ratio: 1;
            position:absolute;
	        border-radius: 50%;
            background-color:var(--black);
            overflow:hidden;

	        &>div:nth-child(1) {
	            position: absolute;
	            height: 16px;
	            width: 20px;
	            background-color: var(--shadowYellow);
	            position: absolute;
	            transform: translate(100px, 115.5px) skewY(-34deg);
	            box-shadow: 0 26px var(--shadowYellow), 0 52px var(--shadowYellow);
	        }

	        &>div:nth-child(2) {
	            position: absolute;
	            height: 16px;
	            width: 100px;
	            background-color: var(--yellow);
	            transform: translate(0px, 122px);
	            box-shadow: 0 25.6px var(--yellow), 0 52px var(--yellow);

	            &:before {
	                content: '';
	                position: absolute;
	                height: 16px;
	                width: 100px;
	                background-color: var(--yellow);
	                transform: translate(120px, -13px);
	                box-shadow: 0 26px var(--yellow), 0 52px var(--yellow);
	            }

	            &:after {
	                content: '';
	                position: absolute;
	                height: 40px;
	                aspect-ratio: 1;
	                background-color: var(--yellow);
	                transform: translate(40px, -82px);
                    border-radius:50%;
	            }
	        }

	    }
	}
</style>
