<script>
	// export let name;
	// import './button.scss';
  	// import Button, {Group, GroupItem, Label, Icon} from '@smui/button';
	// export let name;
	function start() {
		alert('clicked')
	}
	let clicked = 0
</script>

<main>
	<h1>Welcome to yet another Implicit Association Test!</h1>
	<p>The goal of this test is to reveal our inherent gender biases in accordance how we categorise words.</p>
	<p>For more information on this and other tests, visit <a href='https://implicit.harvard.edu/implicit/iatdetails.html'>this website!</a></p>

	<!-- <h1>Welcome!</h1> -->
	<p>In this study, you will be asked to sort words into groups as fast as you can. There will also be some questions examining your beliefs and some standard demographic questions. This should take about 10 minutes for you to complete, to which you will receive a result and an interpretation.</p>	
	<p>The task will assess your automatic associations of words with male and female genders.</p>
	<p>Thanks for trying this out!</p>

	<button on:click={start}>
		Let's Go!
	</button>
	<!-- <Button on:click={() => clicked++} variant="raised"><Label>Let's Go (raised)</Label></Button> -->
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