<script>
	import './button.scss';
  	import Button, {Group, GroupItem, Label, Icon} from '@smui/button';
	// export let name;
	function start() {
		alert('clicked')
	}
	let clicked = 0
	let hotColdAnswers = ['Very warm', 'Moderately warm', 'Slightly warm', 'Neither warm nor cold', 'Slightly cold', 'Moderately cold', 'Very cold']
	let agreeAnswers = ['Strongly agree', 'Moderately agree', 'Slightly agree', 'Neither agree or disagree', 'Slightly disagree', 'Moderately disagree', 'Strongly disagree']
	let trueAnswers = ['Totally true for me', 'Mostly true for me', 'Moderately true for me', 'Somewhat true for me', 'Not true at all for me']
	let genderAnswers = ['Men', 'Women', 'Non-binary', 'None']
</script>

<main>
	<h1>Qustionnaire</h1>
	<!--Questions on beliefs-->
	<p>How warm or cold do you feel towards men?</p>	
	<p>How warm or cold do you feel towards women?</p>
	<p>Men are discriminated against</p>
	<p>women are discriminated against</p>
	<p>I prefer the company of men over women</p>
	<p>I prefer the company of women over men</p>
	<p>I have a sexual preference for</p>
	<p>I have a romantic preference for</p>
	<!--Questions on demographics-->
	<p>What was your sex assigned at birth?</p>
	<p>What is your current gender identity</p>
	<p>Birth year (use date picker)</p>
	<p>What is your race?</p>
	<p>What is your ethnicity?</p>
	<p>How many Implicit Association Tests (IAT) have you performed?</p>
	<p>What is your political identity?</p>
	<p>What is your religious affiliation?</p>
	<p>How religious do you consider yourself to be?</p>
	<p>What is your country of birth?</p>
	<p>What is your country of residence?</p>
	<p>Please indicate what is the highest level of education that you have received</p>
	<p>What is your occupation?</p>

	<!--4 categories: Male, Female, Good, Bad-->


	<button on:click={start}>
		Let's Go!
	</button>
	<Button on:click={() => clicked++} variant="raised"><Label>Let's Go (raised)</Label></Button>

</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>