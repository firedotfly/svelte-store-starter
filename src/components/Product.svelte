<script>
    import BackSVG from './BackSVG.svelte';
</script>


<div id="container" >
    <button class="back-button">
        <BackSVG />
        Back To Catalogue
    </button>
    <main class="catalog">
        <div class="product-image">
            <div class="image-main">
                <img src="" alt="">
            </div>
        </div>
        <div class="product-details">
            <h1 class="product-name"></h1>
            <p class="product-description"></p>
            <hr>
            <div class="product-price">₹ </div>
            <div class="action-buttons">
                <button>Add to Cart</button>
            </div>
        </div>
    </main>
</div>