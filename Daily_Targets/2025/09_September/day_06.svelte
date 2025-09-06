<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--dark: #142932;
		--green: #00d47e;
        background-color: var(--dark);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div {
			position: absolute;
			height: 120px;
			width: 310px;
			background-color: var(--green);
			translate: 0 -55px;
			border-radius: 60px/60px;
			&:before {
				content: '';
				position: absolute;
				height: 190px;
				width: 90px;
				background-color: var(--green);
				translate: 111px 40px;
			}
            &:after{
                content:'';
                position:absolute;
                height: 300px;
                width: 300px;
                background-color:var(--dark);
                clip-path:polygon( 31px 30px, 282px 30px , 282px 90px,140px 90px, 140px 200px, 170px 200px , 170px 90px,31px 90px);
            }
		}
	}
</style>
