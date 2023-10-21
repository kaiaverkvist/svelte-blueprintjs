<script>
	import './../styles/app.css';
	import Button from "../../../components/core/Button/Button.svelte";
    import { IntentDanger, IntentNone, IntentPrimary, IntentWarning } from '../../../components/core/intents';
    import Spinner from '../../../components/core/Spinner/Spinner.svelte';
    import ButtonGroup from '../../../components/core/ButtonGroup/ButtonGroup.svelte';
</script>
<main>
	<section>
		<h1>Button</h1>
		<Button icon="refresh">Primary button</Button>
		<Button icon="share" disabled>Disabled button</Button>
		<Button icon="play" active>Active button</Button>
		<Button loading>Loading button</Button>
		<Button icon="document" minimal>Minimal button</Button>
		<hr>
		<Button intent={IntentNone}>Default button</Button>
		<Button intent={IntentPrimary}>Primary button</Button>
		<Button intent={IntentWarning}>Warning button</Button>
		<Button intent={IntentDanger}>Danger button</Button>
	</section>

	<section>
		<h1>Button group</h1>
		<ButtonGroup>
			<Button icon="refresh">A button</Button>
			<Button icon="plus">Other button</Button>
		</ButtonGroup>
	</section>

	<section>
		<h1>Spinner</h1>
		<div style="display:flex; gap: 1rem;">
			<Spinner size=30 />
			<Spinner size=30 intent={IntentPrimary} />
			<Spinner size=30 intent={IntentWarning} />
			<Spinner size=30 intent={IntentDanger} />
		</div>
	</section>
</main>

<style>
	main {
		padding: 2rem;
	}
</style>