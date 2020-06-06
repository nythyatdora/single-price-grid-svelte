<script>
	import Button from './Button.svelte'
</script>

<main>
	<div class="wrapper">
		<div class="header">
			<h3 class="txt-primary-1">Join our community</h3>
			<h4 class="txt-primary-2">
				30-day, hassie-free money back gurantee
			</h4>
			<p class="txt-neutral-2">
				Gain access to our full library of tutorials along with expert
				code reviews. <br />Perfect for any developers who are serious
				about honing their skills.
			</p>
		</div>
		<div class="body">
			<div class="left bg-primary-1">
				<h4 class="txt-white">Monthly Subscription</h4>
				<div class="d-flex">
					<span class="font-size-big font-weight-700 txt-white"
						>$29</span
					>
					<span class="align-self-center pd-lf-sm txt-neutral-1"
						>per month</span
					>
				</div>
				<p class="txt-white txt-sm pd-bt-md">
					Full access for less than $1 a day
				</p>
				<Button>Sign Up</Button>
			</div>
			<div class="right bg-neutral-2">
				<h4 class="txt-neutral-1">Why Us</h4>
				<p class="txt-neutral-1 txt-sm">
					Tutorials by industry experts Peer & expert code review<br />
					Coding exercises Access to our GitHub Repos Community
					forum<br />
					Flashcard decks New videos every week
				</p>
			</div>
		</div>
	</div>
</main>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Karla&display=swap');

	:root {
		--primary-1: hsl(179, 62%, 43%);
		--primary-2: hsl(71, 73%, 54%);
		--neutral-1: hsl(204, 43%, 93%);
		--neutral-2: hsl(218, 22%, 67%);
	}

	.txt-white {
		color: white;
	}

	.txt-primary-1 {
		color: var(--primary-1);
	}

	.bg-primary-1 {
		background-color: var(--primary-1);
	}

	.txt-primary-2 {
		color: var(--primary-2);
	}

	.bg-primary-2 {
		background-color: var(--primary-2);
	}

	.txt-neutral-1 {
		color: var(--neutral-1);
	}

	.bg-neutral-1 {
		background-color: var(--neutral-1);
	}

	.txt-neutral-2 {
		color: var(--neutral-2);
	}

	.bg-neutral-2 {
		background-color: var(--neutral-2);
	}

	body {
		font-size: 16px;
		font-family: 'Karla', sans-serif;
	}

	.font-weight-400 {
		font-weight: 400;
	}

	.font-weight-700 {
		font-weight: 700;
	}

	.font-size-big {
		font-size: 2rem;
	}
	.wrapper {
		width: 680px;

		background-color: white;
		border-radius: 6px;

		box-shadow: 0 10px 20px rgba(0, 0, 0, 0.19),
			0 6px 6px rgba(0, 0, 0, 0.23);
	}

	.header {
		margin: 3rem;
	}

	.body {
		display: grid;
		grid-template-columns: repeat(2, 1fr);
	}

	.left {
		padding: 2rem 2rem 2rem 3rem;
	}

	.right {
		padding: 2rem 3rem 2rem 2rem;
	}

	.d-flex {
		display: flex;
	}

	.align-self-center {
		align-self: center;
	}

	.pd-lf-sm {
		padding-left: 0.6rem;
	}

	.pd-bt-md {
		padding-bottom: 1.2rem;
	}

	.txt-sm {
		font-size: 15px;
	}

	main {
		display: flex;
		width: 100%;
		height: 100%;
		background-color: var(--neutral-1);

		justify-content: center;
		align-items: center;
	}

	p {
		letter-spacing: 0.03rem;
		line-height: 1.4rem;
	}

	@media screen and (max-width: 375px) {
		.body {
			display: grid;
			grid-template-columns: repeat(1, 1fr);
		}
	}
</style>
