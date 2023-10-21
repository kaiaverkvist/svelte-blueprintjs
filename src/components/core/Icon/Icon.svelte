<script>
    import { IntentNone } from "../intents";

    export let icon = "trash"
    export let size = "standard"
    export let intent = IntentNone;
</script>

<span class="bp5-icon-{size} bp5-icon-{icon} {intent ? 'bp5-intent-' + intent : ''}"></span>