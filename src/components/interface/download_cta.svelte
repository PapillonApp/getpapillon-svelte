<script>
  import PapillonDownload from '$lib/icons/download.svg';
</script>

<a href="#" class="button_download_cta" aria-label="Télécharger Papillon">
  <img src={PapillonDownload} alt="Télécharger" />
  <p class="button_download_cta_text">
    Télécharger
  </p>
  <p class="button_download_cta_subtext">
    v6
  </p>
</a>

<style>
  .button_download_cta {
    display: flex;
    padding: 8px 12px;
    align-items: center;
    gap: 11px;
    border-radius: 80px;
    border: 1px solid var(--text-color);
    color: var(--text-color);
    text-decoration: none;
    width: fit-content;
  }

  .button_download_cta:hover {
    background-color: rgba(var(--text-color-rgba), 0.2);
  }

  .button_download_cta img {
    height: 20px;
  }

  .button_download_cta_text {
    font-size: 1em;
    font-weight: 500;
  }

  .button_download_cta_subtext {
    font-size: 0.9em;
    font-weight: 400;
    opacity: 0.5;
  }
</style>