<script setup>
</script>

<template>
<header>
	<div>
		<img alt="" src=# />
		<p>Frontend Design & Development</p>
	</div>
	<div>
		<nav>
			<h2>Menu</h2>
			<ul>
					<li>
						<a href=# target="_self"> sprint 3 </a>
					</li>
			</ul>
		</nav>
	</div>
</header>
</template>

<style scoped>
	a {
		text-decoration: none;
		margin-left: .3rem;
		padding: 0 1.5em;
	}

	header div {
		display: flex;
		max-width: 95vw;
		flex-wrap: nowrap;
		align-items: baseline;
		justify-content: space-between;
		margin-left: 2em;
	}

	header div:first-of-type {
		justify-content: start;
		align-items: center;
		padding-bottom: 1em;
	}

	header img {
		height: 90px;
		margin-top: 0.2em;
		margin-right: -1.7em;
	}

	header p {
		color: #050542;
		border-left: 1px solid #050542;
		padding: 0 1em;
		font-size: 1.2em;
		letter-spacing: -0.03em;
	}

	nav {
		position: relative;
		font-size: 0.8rem;
		background-color: #ECECEC;
		color: #050542;
		border-radius: 15px 15px 0 0;
		margin-top: 1em;
		margin-inline: auto;
	}

	nav h2 {
		padding: -.25em;
	}

	nav::before {
		content: '';
		position: absolute;
		width: 1.5em;
		aspect-ratio: 1;
		left: -1.5em;
		border-radius: 0 0 50% 0;
		bottom: 0;
		box-shadow: 0.5em 0.5em 0 0 #ECECEC;
	}

	nav::after {
		content: '';
		position: absolute;
		width: 1.5em;
		aspect-ratio: 1;
		right: -1.5em;
		border-radius: 0 0 0 50%;
		bottom: 0;
		box-shadow: -0.5em 0.5em 0 0 #ECECEC;
	}
	nav ul {
		display: flex;
		font-weight: 500;
		padding: 0 4em;
		gap: 1em;
	}

	@media (max-width: 750px) {
		nav ul {
			font-size: 0.75em;
		}
	}

	@media (min-width: 22em) {
		nav {
			font-size: 1rem;
		}
	}

	a {
        position: relative;
        z-index: 1;
        padding: .75rem;
        background-color: #fff;
        border-radius: 10px;
		border: 1px solid #050542;
        color: #050542;
        font-weight: 700;
        text-decoration: none;
    }
	
	li a:focus-visible, li a:hover {
		background-color: #fffc86;
		right: 1px;
        top: 2px;
	}

	li a:focus-visible::before, li a:hover::before {
		background-color: #b1b073;
		right: 2px;
    	top: 2px;
	}

	li a.active{
		background-color: #66e5bf;
		color: #050542;
	}

	li a.active::before {
		background-color: #56ad93;
		color: #050542;
	}

	li a.active:hover, li a.active:focus-visible {
		background-color: #fffc86;
		color: #050542;
	}
	li a.active:hover::before, li a.active:focus-visible::before {
		background-color: #b1b073;
		color: #050542;
	}

    li a::before {
        content: "";
        z-index: -10;
        position: absolute;
        width: 100%;
        height: 100%;
        border: 1px solid #050542;
        background-color: #ECECEC;
        border-radius: 10px;
        color: #050542;
        right: 4px;
        top: 4px;
	}
</style>