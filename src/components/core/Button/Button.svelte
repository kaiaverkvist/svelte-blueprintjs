<script>
    import { IntentNone } from "../intents.js";
    import Spinner from "../Spinner/Spinner.svelte";

    export let icon = null;
    export let disabled = false;
    export let active = false;
    export let loading = false;
    export let minimal = false;
    export let outlined = false;
    export let fill = false;
    export let intent = IntentNone;
</script>

<button
    class="bp5-button {intent ? 'bp5-intent-' + intent : ''}"
    class:bp5-disabled={disabled || loading}
    class:bp5-active={active}
    class:bp5-loading={loading}
    class:bp5-minimal={minimal}
    class:bp5-outlined={outlined}
    class:bp5-fill={fill}
    {disabled}
    type="button"
>
    {#if icon}
        <span class="bp5-icon bp5-icon-{icon}" />
    {/if}
    {#if loading}
        <Spinner />
    {/if}
    <span class="bp5-button-text">
        <slot />
    </span>
</button>
