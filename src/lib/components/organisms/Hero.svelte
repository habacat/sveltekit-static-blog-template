<script>
	import SparklingHighlight from '$lib/components/molecules/SparklingHighlight.svelte';
	import FeaturesIcon from '$lib/icons/features.svelte';
	import GitHubIcon from '$lib/icons/socials/github.svelte';
	import Button from '$lib/components/atoms/Button.svelte';
	import Sparkles from '../atoms/Sparkles.svelte';
</script>

<section id="hero">
	<h1 class="hello">
		<SparklingHighlight color="primary">复旦大学 电子竞技联盟</SparklingHighlight>
	</h1>
	<p class="intro">
		<span class="left"> 带上你的热情，</span>
		<span class="right">和我们一起踏上电竞之旅！ </span>
	</p>
	<!-- <div class="ctas">
		<Sparkles>
			<Button href="https://github.com/matfantinel/sveltekit-static-blog-template">
				<GitHubIcon slot="icon" />
				Source Code
			</Button>
		</Sparkles>
		<Button color="primary" href="https://histoire-sveltekit-static-blog-template.vercel.app/">
			<FeaturesIcon slot="icon" />
			Components
		</Button>
	</div> -->
</section>

<style lang="scss">
	@import '$lib/scss/breakpoints.scss';

	#hero {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		gap: 15px;
		position: relative;
		padding: 80px 0;

		@include for-phone-only {
			padding: 40px 0 50px;
		}

		.hello {
			text-align: center;
			font-weight: 500;
			font-size: 3.5rem;
			// width: min(100%, 2200px);
			display: flex;
			flex-direction: column;
			font-family: sans-serif;
			font-kerning: auto;
			justify-content: space-between;
			@include for-phone-only {
				font-weight: 200;
				font-size: 2rem;
			}
		}

		.intro {
			font-weight: 500;
			font-size: 1.2rem;
			width: min(100%, 440px);
			display: flex;
			flex-direction: column;
			font-style: oblique;
			.left {
				text-align: left;
			}
			.right {
				text-align: right;
			}

			@include for-phone-only {
				font-size: 1.2rem;
				justify-content: center;
				flex-direction: column;
				margin-left: 10%;
				margin-right: 10%;
				// display: none;
			}
		}

		.ctas {
			display: flex;
			flex-wrap: wrap;
			align-items: center;
			justify-content: center;
			gap: 10px;
			width: 100%;
		}
	}
</style>
