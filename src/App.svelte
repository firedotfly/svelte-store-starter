<script>
	import CartSVG from './components/Cart.svelte';

	let results = [], filters = [];

	const load = async () => {
		const res = await fetch(`https://raw.githubusercontent.com/firedotfly/svelte-store-starter/main/src/products.json`);
		const results = await res.json();
 	}
	load();

</script>

<nav class="navbar" role="navigation" aria-label="navigation">
	<a class="brand-logo" href="/">Some<span class="brand-color">Bakery</span></a>
	<ul>
		<li>About</li>
		<li>Offers</li>
		<li>Stores</li>
		<li>Catering</li>
	</ul>
	<button>
		<CartSVG />
	</button>
</nav>

<div id="app">
	<div class="catalogue-wrapper">
		<div class="catalogue-type">
			<h2>Bakery Items</h2>
		</div>
		<div>
			<ul>
				<li></li>
			</ul>
		</div>
		<div class="catalogue-display">
			<h1>Home</h1>
			<div class="catalogue-total"></div>
			<div class="catalogue">
				<div class="product">
					<img src="" loading="lazy" alt="">
					<div class="product-price"></div>
					<p class="product-name"></p>
				</div>
			</div>
		</div>
	</div>
</div>
