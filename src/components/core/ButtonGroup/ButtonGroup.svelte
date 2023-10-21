<script>
    export let large = false
    export let minimal = false
    export let vertical = false
</script>

<div class="bp5-button-group"
    class:bp5-large={large}
    class:bp5-minimal={minimal}
    class:bp5-vertical={vertical}
>
    <slot />
</div>