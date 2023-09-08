<script>
	import FooterWave from '$lib/icons/footer-wave.svelte';
	import Socials from '$lib/components/molecules/Socials.svelte';
	import ThemeToggle from '$lib/components/molecules/ThemeToggle.svelte';
	import RssLink from '$lib/components/atoms/RssLink.svelte';
</script>

<footer>
	<div class="wave">
		<FooterWave />
	</div>
	<div class="content">
		<div class="copyright">
			版权所有：复旦电子竞技联盟 <a
				href="https://fantinel.dev?utm_source=site-template"
				target="_blank"
				rel="noopener noreferrer">Designed by 秋声.</a
			>.
		</div>
		<div class="credits">
			<p>凿破苍苔地，偷他一片天</p>
			<p>白云生镜里，明月落阶前</p>
		</div>
		<!-- <div class="credits">白云生镜里，明月落阶前。</div> -->
		<div class="socials">
			<!-- <Socials />
			<RssLink />
			<ThemeToggle /> -->
		</div>
	</div>
</footer>

<style lang="scss">
	footer {
		height: 340px;
		width: 100%;
		background: linear-gradient(60deg, var(--color--waves-start) 0%, var(--color--waves-end) 100%);
		display: grid;
		grid-template-rows: 120px 1fr;

		.content {
			display: flex;
			flex-direction: column;
			align-items: center;
			justify-content: center;
			gap: 15px;
			font-weight: 600;
			text-align: center;

			.credits {
				font-weight: 400;
				font-size: 90%;
				color: var(--color--text-shade);
			}

			.socials {
				display: flex;
				align-items: center;
				gap: 20px;
			}
		}

		a {
			&:hover {
				filter: drop-shadow(0px 0px 3px var(--color--primary));
			}
		}
	}
</style>
