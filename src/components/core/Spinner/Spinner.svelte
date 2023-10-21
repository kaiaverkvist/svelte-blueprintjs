<script>
    import { IntentNone } from "../intents";

    export let size = 20;
    export let value = null;
    export let intent = IntentNone;

</script>

<div class="bp5-spinner {intent ? 'bp5-intent-' + intent : ''}">
    <div class="bp5-spinner-animation">
        <svg width={size} height={size} stroke-width="8.00" viewBox="1.00 1.00 98.00 98.00"><path class="bp5-spinner-track" d="M 50,50 m 0,-45 a 45,45 0 1 1 0,90 a 45,45 0 1 1 0,-90"></path><path class="bp5-spinner-head" d="M 50,50 m 0,-45 a 45,45 0 1 1 0,90 a 45,45 0 1 1 0,-90" pathLength="280" stroke-dasharray="280 280" stroke-dashoffset="210"></path></svg>
    </div>
</div>