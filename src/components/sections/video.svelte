<div class="section">
  <div class="width">
    <div class="section-header">
      <h2>
        Vidéo de présentation
      </h2>
      <p>
        Découvrez en vidéo les fonctionnalités principales qui font de Papillon une application géniale à utiliser au quotidien.
      </p>
      <br />
      <p style="opacity: 0.5;">
        Emploi du temps facile d'accès, devoirs synchronisés, historique des moyennes générales, détail des notes, notifications, personnalisation de l'application et du profil, sélection de la couleur des matières, et bien plus encore.
      </p>
    </div>

    <video controls class="video">
      <source src="/papillon_v6_intl_h264.mp4" type="video/mp4">
      Votre navigateur ne supporte pas la vidéo.
    </video>
  </div>
</div>

<style>
  .section {
    background-color: var(--primary-color);
  }

  .section .width {
    flex-direction: row;
    justify-content: space-between;
  }

  .section-header {
    width: 100%;
  }

  .video {
    flex: 1;
    width: 100%;
    max-width: 600px;
    height: auto;
    border-radius: 8px;
    border: 1px solid rgba(var(--text-color-rgba), 0.3);
  }

  @media (max-width: 1000px) {
    .section .width {
      flex-direction: column;
    }
  }
</style>