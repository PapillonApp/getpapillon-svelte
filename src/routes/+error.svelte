<script>
	import { page } from '$app/stores';
  import Navbar from '../components/interface/navbar.svelte';

  console.log($page);
</script>

<Navbar />
<div class="section">
  <div class="width">
    <div class="section-header">
      <h2>
        Erreur {$page.status} : {$page.error.message}
      </h2>
      <p>
        Cette page n'existe pas ou est inaccessible.
      </p>
    </div>
    <div>
      <a href="/" style="color: var(--text-color);">Retour à l'accueil</a>
    </div>
  </div>
</div>