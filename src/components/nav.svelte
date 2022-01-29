<nav>
	<div class="logo">
		<h4>Best movies store</h4>
	</div>

	<ul class="navi-links">
		<li>
			<a href="#home"> Home </a>
		</li>
		<li>
			<a href="#about"> About </a>
		</li>
		<li>
			<a href="#resume"> Store </a>
		</li>
		<li>
			<a href="#portfolio"> Contact us </a>
		</li>
		<li>
			<a href="#blog"> Blog </a>
		</li>
	</ul>
</nav>

<style>
	nav {
		position: fixed;
		display: flex;
		justify-content: space-around;
		align-items: center;
		font-family: 'Fira Mono', monospace;
		min-height: 9vh;
		width: 100%;
		background-color: rgb(0, 0, 0);
		font-weight: bold;
		transition: 0.6s;
		z-index: 1000;
	}

	.logo {
		color: aliceblue;
		text-transform: uppercase;
		letter-spacing: 5px;
		font-size: 1.4rem;
		margin-left: 10vw;
	}

	.navi-links {
		display: flex;
		justify-content: space-around;
		width: 35%;
	}

	.navi-links li {
		list-style: none;
	}

	.navi-links a {
		color: aliceblue;
		text-decoration: none;
		letter-spacing: 3px;
		font-weight: bold;
		font-size: 1.2rem;
	}
</style>
