<script>
  import Navbar from "../interface/navbar.svelte";
  import DownloadCta from "../interface/download_cta.svelte";

  import Phones from '$lib/assets/phones.png';
</script>

<div class="header">
  <Navbar />
  
  <div class="width content">
    <div class="text">
      <p class="title fixel">
        Votre vie scolaire, avec une expérience d'utilisation unique.
      </p>
      <p class="description">
        Papillon est un client libre, open-source et développé par une communauté d’élèves pour l’ensemble de vos services de vie scolaire.
      </p>
      <DownloadCta />
      <p class="conditions">
        En téléchargeant l’app, vous acceptez les <a href="https://docs.getpapillon.xyz/documents/terms-of-service/">conditions d’utilisation</a> et la <a href="https://docs.getpapillon.xyz/documents/privacy-policy/">politique de confidentialité</a>
      </p>
    </div>
    <enhanced:img src='../../lib/assets/phones.png' alt="Capture d'écran de l'application" />
  </div>
</div>

<style>
  .header {
    background: radial-gradient(207.16% 62.04% at 26.33% 83.45%, rgba(50, 171, 142, 0.20) 0%, rgba(20, 69, 57, 0.00) 100%), radial-gradient(121.18% 90.28% at 73.42% 26.76%, rgba(50, 171, 142, 0.50) 0%, rgba(20, 69, 57, 0.00) 100%), #313747;
    height: 420px;

    overflow: hidden;
  }

  .content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 40px;
    padding: 0;
  }

  .text {
    display: flex;
    flex-direction: column;
    gap: 20px;
    max-width: 400px;
  }

  .title {
    font-size: 2em;
    line-height: 1em;
    font-weight: 600;
    color: var(--text-color);
  }

  .description {
    font-size: 1em;
    line-height: 1.1em;
    font-weight: 400;
    color: var(--text-color);
  }

  .conditions {
    font-size: 0.8em;
    line-height: 1.1em;
    font-weight: 400;
    color: rgba(var(--text-color-rgba), 0.5);
  }

  .conditions a {
    color: var(--text-color);
    text-decoration: underline;
  }

  img {
    margin-right: -50px;
    width: 618px;
    height: 348px;
  }

  @media (max-width: 950px) {
    .header {
      height: fit-content;
    }

    .content {
      flex-direction: column;
      gap: 20px;
      padding: 0px;
      padding-bottom: 0px;
      margin-top: 20px;
    }

    img {
      margin-right: 0;
      width: 618px;
      height: 348px;
    }

    .title {
      font-size: 1.7em;
    }
  }
</style>
