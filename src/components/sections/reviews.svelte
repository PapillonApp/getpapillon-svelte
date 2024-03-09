<script>
  import Stars from '$lib/icons/stars.svg';
</script>

<div class="section">
  <div class="width">
    <div class="section-header">
      <h2>
        Utilisé et apprécié par des milliers d'utilisateurs
      </h2>
      <p>
        Papillon est l'application alternative de vie scolaire la plus utilisée et les utilisateurs en sont satisfaits. Voyez par vous-même ce qu'ils en disent.
      </p>
    </div>

    <div class="reviews">

      <div class="review">
        <div class="review-title">
          <p class="review-title-text">
            Un changement de vie
          </p>
          <img src={Stars} alt="Note de 5 étoiles" class="review-stars" />
        </div>
        <div class="review-user">
          <p class="review-user-name">
            Timo FEB.
          </p>
          <div class="review-user-separator"></div>
          <p class="review-user-date">
            19 oct 2023
          </p>
        </div>
        <p class="review-content">
          Grâce à cette application magique, la gestion de mon emploi du temps a évolué. Pourquoi ? Parce que l’application Papillon est passée par là...
        </p>
      </div>

      <div class="review">
        <div class="review-title">
          <p class="review-title-text">
            Super appli
          </p>
          <img src={Stars} alt="Note de 5 étoiles" class="review-stars" />
        </div>
        <div class="review-user">
          <p class="review-user-name">
            Dreiouchdu92
          </p>
          <div class="review-user-separator"></div>
          <p class="review-user-date">
            30 sept. 2023
          </p>
        </div>
        <p class="review-content">
          Depuis la mise à jour c’est vraiment devenu la meilleure application, elle est très stable et marche même hors connexion !
        </p>
      </div>

      <div class="review">
        <div class="review-title">
          <p class="review-title-text">
            Un changement de vie
          </p>
          <img src={Stars} alt="Note de 5 étoiles" class="review-stars" />
        </div>
        <div class="review-user">
          <p class="review-user-name">
            et apres ?
          </p>
          <div class="review-user-separator"></div>
          <p class="review-user-date">
            21 nov 2023
          </p>
        </div>
        <p class="review-content">
          Bravo les gars c’est trop bien, PRONOTE en mode sombre, avec couleurs personnalisable, accueil aussi etc. Bref une dinguerie.
        </p>
      </div>

    </div>
  </div>
</div>

<style>
  .reviews {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
  }

  .review {
    flex: 1;
    display: flex;
    padding: 14px 14px;
    flex-direction: column;
    background-color: var(--background-over-100);
    border: 1px solid rgba(var(--text-color-rgba), 0.2);
    border-radius: 8px;
    gap: 4px;
    transition: all 0.28s cubic-bezier(0.2,0,0,1);
  }

  .review:hover {
    border: 1px solid rgba(var(--text-color-rgba), 0.4);
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    transform: translateY(-4px);
  }

  .review-title {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    gap: 4px;
  }

  .review-title-text {
    font-size: 1em;
    font-weight: 600;
    color: var(--text-color);
    margin: 0;
  }

  .review-stars {
    height: 14px;
  }

  .review-user {
    display: flex;
    gap: 10px;
    align-items: center;
  }

  .review-user-name {
    font-size: 0.9em;
    font-weight: 600;
    color: var(--text-color);
    margin: 0;
  }

  .review-user-separator {
    width: 1px;
    height: 16px;
    background-color: rgba(var(--text-color-rgba), 0.5);
  }

  .review-user-date {
    font-size: 0.9em;
    font-weight: 400;
    color: rgba(var(--text-color-rgba), 0.5);
    margin: 0;
  }

  .review-content {
    font-size: 0.9em;
    line-height: 1.2em;
    font-weight: 400;
    color: var(--text-color);
    text-align: left;
  }

  @media (max-width: 900px) {
    .reviews {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 600px) {
    .reviews {
      grid-template-columns: repeat(1, 1fr);
    }
  }
</style>