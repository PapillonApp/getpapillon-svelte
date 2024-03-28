<script>
	import Navbar from '../../components/interface/navbar.svelte';
</script>

<Navbar />
<div class="section">
	<div class="width">
		<div id='load' class="section-header get">
			<h1>
				Prépare-toi à découvrir une révolution !
			</h1>
			<p>
				Nous préparons ton arrivée, tu vas bientôt pouvoir télécharger Papillon.
			</p>
			<div class="loader" style="margin-top: 40px"><div></div><div></div><div></div><div></div></div>
		</div>
		<div id="device-not-found" class="section-header get" style="align-items: flex-start;display: none;">
			<h1>
				Oups, nous n'arrivons pas à déterminer ton appareil.
			</h1>
			<p>
				Sélectionne ton appareil ci-dessous pour télécharger Papillon.
			</p>

			<a style="margin-top: 40px; color: var(--text-color);" href="https://play.google.com/store/apps/details?id=xyz.getpapillon.app">Android</a>
			<a style="margin-top: 10px; color: var(--text-color);" href="https://play.google.com/store/apps/details?id=xyz.getpapillon.app">iOS</a>

			<p style="margin-top: 40px; color: var(--text-color-secondary);">Ton appareil n'est pas listé ? C'est qu'il n'est pas compatible pour le moment avec Papillon !</p>
		</div>
	</div>

	<script>
		let userAgent = navigator.userAgent || navigator.vendor || window.opera;

		if (/android/i.test(userAgent)) {
			window.location.href = 'market://details?id=xyz.getpapillon.app'
		}

		// iOS detection from: http://stackoverflow.com/a/9039885/177710
		if (/iPad|iPhone|iPod/.test(userAgent) && !window.MSStream) {
			window.location.href = 'https://apps.apple.com/fr/app/papillon-lappli-scolaire/id6477761165'
		}
		setTimeout(() => {
			document.getElementById('load').style.display = 'none';
			document.getElementById('device-not-found').style.display = 'flex';
		}, 3000)

	</script>
</div>
