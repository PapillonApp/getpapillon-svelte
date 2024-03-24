<script>
</script>

<div class="section">
  <div class="width">
    <div class="section-header">
      <h2>Pour vous, rien qu’à vous</h2>
      <p>
        Créée par des élèves, l’application se concentre essentiellement sur les fonctionnalités dont vous avez réellement besoin, et y ajoute des options géniales pour faire de Papillon le vôtre.
      </p>
    </div>

    <div class="cards">

      <div class="card card-1">
        <h2>
          Travail à faire
        </h2>
        <p>
          Consultez efficacement vos devoirs, cochez-les et rendez-les de manière synchronisée avec votre établissement.
        </p>
        <enhanced:img src='../../lib/assets/cards_trav.png' alt="Capture d'écran du travail à faire" />
      </div>
      <div class="card card-2">
        <h2>
          Emploi du temps
        </h2>
        <p>
          Un emploi du temps facile et intuitif à utiliser, avec tout ce dont vous avez besoin pour votre journée.
        </p>
        <enhanced:img src='../../lib/assets/cards_edt.png' alt="Capture d'écran de l'emploi du temps" />
      </div>
      <div class="card card-3">
        <h2>
          Détail des notes
        </h2>
        <p>
          Vos notes vous sont importantes, il faut que vous soyez capable de mieux les comprendre avec des analyses.
        </p>
        <enhanced:img src='../../lib/assets/cards_notes.png' alt="Capture d'écran du détail des notes" />
      </div>
    </div>
  </div>
</div>

<style>
  .cards {
    width: 100%;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
  }

  .card {
    display: flex;
    padding: 20px 24px 0px 24px;
    flex-direction: column;
    align-items: center;
    gap: 14px;
    border-radius: 8px;
    border: 1px solid rgba(255, 255, 255, 0.15);
    transition: all 0.28s cubic-bezier(0.2,0,0,1);
    overflow: hidden;
  }

  .card * {
    user-select: none;
  }

  .card:hover {
    border: 1px solid rgba(255, 255, 255, 0.35);
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    transform: translateY(-4px);
  }

  .card h2 {
    font-size: 1.15em;
    font-weight: 600;
    color: #FFFFFF;
    margin: 0;
  }

  .card p {
    font-size: 0.9em;
    line-height: 1.2em;
    font-weight: 400;
    color: #FFFFFF;
    text-align: center;
  }

  .card img {
    width: 254px;
    height: 236px;
    margin-top: 10px;
    margin-bottom: -5px;
    transition: all 0.28s cubic-bezier(0.2,0,0,1);
  }

  .card:hover img {
    transform: scale(1.05);
    filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 1));
  }

  .card-1 {
    background: linear-gradient(142deg, rgba(255, 255, 255, 0.00) 53.08%, rgba(255, 255, 255, 0.05) 53.08%, rgba(153, 153, 153, 0.05) 77.86%), linear-gradient(297deg, rgba(50, 171, 142, 0.35) -6.38%, rgba(20, 69, 57, 0.00) 86.04%), #363C4E;
  }

  .card-2 {
    background: linear-gradient(142deg, rgba(255, 255, 255, 0.00) 53.08%, rgba(255, 255, 255, 0.05) 53.08%, rgba(153, 153, 153, 0.05) 77.86%), linear-gradient(235deg, rgba(202, 104, 255, 0.35) 1.62%, rgba(202, 104, 255, 0.00) 87.07%), #363C4E;
  }

  .card-3 {
    background: linear-gradient(142deg, rgba(255, 255, 255, 0.00) 53.08%, rgba(255, 255, 255, 0.05) 53.08%, rgba(153, 153, 153, 0.05) 77.86%), linear-gradient(349deg, rgba(21, 108, 214, 0.35) -24.07%, rgba(21, 108, 214, 0.00) 79.53%), #363C4E;
  }

  @media (max-width: 950px) {
    .cards {
      grid-template-columns: repeat(1, 1fr);
      gap: 20px;
    }
  }
</style>
