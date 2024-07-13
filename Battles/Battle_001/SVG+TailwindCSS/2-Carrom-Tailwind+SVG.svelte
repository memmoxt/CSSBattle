<div class="main">
    <svg viewBox="0 0 100 75" class="h-[300px] w-[400px] absolute">
        {#each Array(9) as _,i}
            <line x1="{10 * (i + 1)}" y1="0" x2="{10 * (i + 1)}" y2="100" class="stroke-red-500 stroke-[0.1px]"></line>
            <line x1="0" y1="{10*(i +1)}" x2="100" y2="{10*(i + 1)}" class="stroke-red-500 stroke-[0.1px]"></line>
        {/each}

        <symbol id="square">
            <rect height="12.5" width="12.5" class="fill-[var(--amber)]"></rect>
        </symbol>

        <rect x="0" y="0" height="75" width="100" class="fill-[var(--brown)]"></rect>
    </svg>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --amber:#fdc57b;
        --brown:#62374e;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>

