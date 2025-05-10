<div class="main">
	<div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
    <div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--purple: #594c94;
		--white: #f9ddc6;
        background-color:var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div {
			position: absolute;
			height: 160px;
			width: 320px;
			background-color: transparent;
			display: grid;
			column-gap:20px;
			grid-template-columns: 40px 60px 40px 60px 40px;
			grid-template-rows: 100px;
			& > div:nth-child(odd) {
				background-color: var(--white);
			}
			& > div:nth-child(even) {
				background-color: var(--white);
                height:60px;
                aspect-ratio:1;
                border-radius:50%;
			}
		}
        &>div:nth-child(2){
            position:absolute;
            height:40px;
            width:320px;
            background-color:var(--white);
            transform: translate(0px,60px);
        }
	}
</style>

