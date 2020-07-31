<nav>
	<ul>
		<li><a href="hello">hello</a></li>
		<li><a href="world">world</a></li>
		<li><a href="svelte">svelte</a></li>
		<li><a href="sapper">sapper</a></li>
	</ul>
</nav>

<style>
	nav {
		border-bottom: 1px solid rgba(255,62,0,0.1);
		font-weight: 300;
		padding: 0 1em;
	}

	ul {
		margin: 0;
		padding: 0;
	}

	/* clearfix */
	ul::after {
		content: '';
		display: block;
		clear: both;
	}

	li {
		display: block;
		float: left;
	}

	a {
		padding: 1em 0.5em;
		display: block;
	}
</style>
