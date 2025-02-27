<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--dark: #183539;
		--light: #46ba67;
        background-color:var(--dark)
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		column-gap: 60px;
		& > div {
			position: absolute;
			height: 250px;
			aspect-ratio: 1;
			background-color: var(--dark);
			box-shadow: 0 0 0 30px var(--light);
			border-radius: 50%;
			top: -204px;
			&:before {
				content: '';
				position: absolute;
				background-color: var(--light);
				left: 74px;
				top: 204px;
				height: 300px;
				width: 101px;
			}
			&:after{
                position: absolute;
				content:'';
                background-color:var(--light);
                top:300px;
                left:-1px;
                height:30px;
                width:266px;
			}
		}
	}
</style>

