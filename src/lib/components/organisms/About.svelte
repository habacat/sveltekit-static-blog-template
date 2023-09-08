<script>
	import SparklingHighlight from '$lib/components/molecules/SparklingHighlight.svelte';
	import Socials from '$lib/components/molecules/Socials.svelte';
	import Image from '../atoms/Image.svelte';
</script>

<section id="about">
	<div class="info">
		<h2>欢迎关注 复旦电子竞技联盟</h2>
		<p><SparklingHighlight color="secondary">感谢每一个热爱电竞的你！</SparklingHighlight></p>
		<p>使用微信扫码二维码加入电竞社核心社群，校内的游戏群聊都在里面哦~</p>
		<p />
		<div class="socials">
			<!-- <span>Socials:</span> -->
			<!-- <Socials /> -->
		</div>
	</div>
	<div class="image">
		<Image src="/qrcode.png" alt="logo" />
		<p />
		⁣⁣⁣⁣　⁣⁣⁣⁣　⁣⁣⁣
		<Image src="/sample-image.png" alt="logo" />
	</div>
	<p />
	<!-- <h2>复旦大学电子竞技联盟微信公众号</h2> -->
</section>

<style lang="scss">
	@import '$lib/scss/breakpoints.scss';

	#about {
		position: relative;
		grid-template-columns: 500px 250px;
		align-items: center;
		justify-content: space-between;
		padding-bottom: 50px;
		font-family: sans-serif;
		display: flex;
		flex-direction: column;

		@include for-phone-only {
			grid-template-columns: 1fr;
			justify-items: center;
			gap: 20px;
		}

		.info {
			display: flex;
			// flex-direction: column;
			gap: 10px;
			font-family: Microsoft YaHei;
			display: flex;
			text-align: center;
			flex-direction: column;
			h2 {
				@include for-phone-only {
					text-align: center;
					font-family: sans-serif;
					display: flex;
					flex-direction: column;
				}
			}

			p {
				@include for-phone-only {
					text-align: justify;
				}
			}

			@include for-phone-only {
				gap: 20px;
			}
		}

		.socials {
			display: flex;
			align-items: center;
			gap: 15px;

			@include for-phone-only {
				justify-content: center;
				margin-bottom: 10px;
				span {
					display: none;
				}
			}
		}

		.image {
			width: 300px;
			height: 300px;
			display: flex;
			justify-content: center; /* 居中对齐图片 */
			margin: auto;
		}
	}
</style>
