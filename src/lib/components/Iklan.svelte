<script>
	import { dev } from '$app/environment';
	import { getContext } from 'svelte';
	import { isMobile } from '$lib/stores/app-store';

	export let type = '';
	export let head = false;

	const showAd = getContext('showAd');

	// onMount(() => {
	// 	if (type !== 'banner') return;
	// 	(window.adsbygoogle = window.adsbygoogle || []).push({});
	// 	return;
	// });
</script>

{#if $showAd}
	{#if type === 'banner'}
		<!-- <ins
		class="adsbygoogle"
		style="display:block"
		data-ad-client="ca-pub-1874822310102113"
		data-ad-slot="6827309798"
		data-ad-format="auto"
		data-full-width-responsive="true"
	/> -->
	{/if}

	{#if head && !dev}
		<!-- <script src="https://adncdnend.azureedge.net/adnimation/agustinusyohannes.js"></script> -->

		<!-- Autotag -->
		<!-- Autotag -->
		<!-- Autotag -->
		<script
			data-cfasync="false"
			type="text/javascript"
			data-adel="atag"
			src="//acacdn.com/script/atg.js"
			czid="v1xd6wvvpe"
		></script>
		<!-- Autotag -->

		{#if !$isMobile}
			<!-- PopAds -->
			<!-- PopAds -->
			<!-- PopAds -->
			<script
				type="text/javascript"
				src="//pl17416355.profitablecpmgate.com/3e/70/98/3e7098724a8a6321d737e1bd39d9ffed.js"
			></script>
			<!-- <script
				src="https://hdbkell.com/xsoi4.js"
				charset="utf-8"
				async
				data-cfasync="false"></script> -->
			<!-- PopAds -->

			<!-- In-Push Page -->
			<!-- In-Push Page -->
			<script
				type="text/javascript"
				src="//pl17419889.profitablecpmgate.com/fb/35/45/fb3545e433a3f40f53c83f80f24037ec.js"
			></script>
			<!-- In-Push Page -->
		{/if}
	{/if}
{/if}
