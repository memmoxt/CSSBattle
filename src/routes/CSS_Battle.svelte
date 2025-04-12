<div class="main">
	<div></div>
</div>

<style>
    * {
    margin: 0;
    padding: 0;
    box-sizing: content-box;
    --yellow: #e3cc9e;
    --red: #995757;
    --white: #ffffff;
    --dark: #6c3232;
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

    &>div {
        position: absolute;
        height: 180px;
        width: 300px;
        background-color: var(--red);

        &:before {
            position: absolute;
            content: '';
            height: 40px;
            width: 300px;
            background-color: var(--red);
            bottom: -20px;
            border-radius: 50%;
            box-shadow: 0 -180px var(--white);
        }

        &:after {
            position: absolute;
            content: '';
            height: 20px;
            width: 140px;
            background-color: var(--dark);
            border-radius: 50%;
            transform: translate(80px, -10px);
        }
    }

}

</style>
