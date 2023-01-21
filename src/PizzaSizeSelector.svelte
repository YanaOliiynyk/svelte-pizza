<script>

    import {onMount} from 'svelte'
    export let size = [];

    let selectedValue =size[0].value;

    $:windowPosition = getPosition(selectedValue)

    function getPosition(selectedValue){
        let value = size.findIndex(fn => {
            if(fn.value == selectedValue){
                return true;
            }
        });

        return (33*value).toString() + "%";
    }

</script>


<div class="selector">
    <div class="type"></div>
    <div class="size">
        <span class="window" style ="left: {windowPosition}"></span>
        {#each size as item}
        <label>
            <input type="radio" bind:group={selectedValue} value={item.value} name={item.name}>
            20 cm
        </label>
        {/each}
    </div>
</div>