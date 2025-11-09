<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #6f9893;
		--white: #d9d9d9;
		--black: #394257;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
        background-color: var(--green);

		& > div {
			--value_for_1: 50px;
			border-top: var(--value_for_1) solid var(--black);
			border-right: var(--value_for_1) solid var(--black);
			border-bottom: var(--value_for_1) solid var(--black);
			border-left: var(--value_for_1) solid var(--black);
			transform: rotate(45deg);
			&:before,
			&:after {
				--value_for: 136px;
				content: '';
				position: absolute;
				transform: rotate(-45deg);
				translate: -145px -60px;
				border-top: var(--value_for) solid transparent;
				border-right: var(--value_for) solid var(--white);
				border-bottom: var(--value_for) solid transparent;
				border-left: 0px solid transparent;
			}
			&:after {
				transform: rotate(135deg);
				translate: 8px -212px;
			}
		}
	}
</style>
