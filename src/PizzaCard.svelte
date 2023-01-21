<script>
    import PizzaSizeSelector from "./PizzaSizeSelector.svelte";

    export let image = '';
    export let name = 'Pizza';
    export let price = 100;

    export let size =[];
</script>

<div class="pizza-card">
    <div class="img">
        <img src="image" alt="X">
    </div>
    <div class="name">{name}</div>
    <PizzaSizeSelector />
    <div class="price-block">
        <div class="price">Від {price}</div>
        <div class="button">
            <button class="btn orange">Купити</button>
        </div>
    </div>
</div>