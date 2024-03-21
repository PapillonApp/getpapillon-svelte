<script>
  import { Hand, Palette, ShieldCheck, Bird, MousePointerSquareDashed, BadgeCheck } from 'lucide-svelte';
</script>

<div class="section">
  <div class="width">
    <div class="section-header">
      <h2>Imaginé par tous, pensé pour chacun</h2>
      <p>
        Papillon est imaginé par de nombreux élèves nourris par la volonté de rendre l’éducation numérique libre, meilleure, accessible et toujours évolutive, pour aider tous les élèves à se construire un environnement numérique accessible, gratuit, adapté et à leur image.
      </p>
    </div>

    <div class="features">

      <div class="feature">
        <div class="feature_icon" style="background-color: #B1861A;">
          <Hand size="24" />
        </div>
        <div class="feature_text">
          <p class="feature_title">
            Accessible
          </p>
          <p class="feature_description">
            L’application se doit d’être ouverte à tous, c’est pour cela qu’elle est compatible avec des fonctionnalités d’accessibilité comme les lecteurs d’écran ou les polices dynamiques.
          </p>
        </div>
      </div>

      <div class="feature">
        <div class="feature_icon" style="background-color: #A74AE0;">
          <Palette size="24" />
        </div>
        <div class="feature_text">
          <p class="feature_title">
            Personnalisable
          </p>
          <p class="feature_description">
            Papillon s’adapte à vos goûts et à vos envies. C’est pour cela que de nombreux aspects de l’application sont personnalisables, et de plus en plus d’options le seront à l’avenir.
          </p>
        </div>
      </div>

      <div class="feature">
        <div class="feature_icon" style="background-color: #3C67BB;">
          <ShieldCheck size="24" />
        </div>
        <div class="feature_text">
          <p class="feature_title">
            Sécurité & vie privée
          </p>
          <p class="feature_description">
            Vos données personnelles et scolaires restent en sécurité dans votre appareil et ne le quittent jamais. L’application utilise les mêmes protocoles que votre établissement.
          </p>
        </div>
      </div>

      <div class="feature">
        <div class="feature_icon" style="background-color: #1C979F;">
          <Bird size="24" />
        </div>
        <div class="feature_text">
          <p class="feature_title">
            Libre
          </p>
          <p class="feature_description">
            Le projet Papillon est un logiciel libre, communautaire et open-source que quiconque peut télécharger, modifier, améliorer, repartager et vérifier
          </p>
        </div>
      </div>

      <div class="feature">
        <div class="feature_icon" style="background-color: #9F1C73;">
          <MousePointerSquareDashed size="24" />
        </div>
        <div class="feature_text">
          <p class="feature_title">
            Interface
          </p>
          <p class="feature_description">
            Le design de l’application et son expérience utilisateur s’améliore continuellement pour créer une application intuitive au delà de vos attentes
          </p>
        </div>
      </div>

      <div class="feature">
        <div class="feature_icon" style="background-color: #859F1C;">
          <BadgeCheck size="24" />
        </div>
        <div class="feature_text">
          <p class="feature_title">
            Fonctionnalités
          </p>
          <p class="feature_description">
            Papillon intègre toutes les fonctionnalités dont vous avez besoin, pour que vous puissiez vous passer des applications traditionnelles.
          </p>
        </div>
      </div>

    </div>
  </div>
</div>

<style>
  .section {
    background-color: var(--background-over-100);
  }

  .features {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
  }

  .feature {
    flex: 1;
    display: flex;
    padding: 14px 14px;
    flex-direction: row;
    background-color: var(--background-over-200);
    border: 1px solid rgba(var(--text-color-rgba), 0.2);
    border-radius: 8px;
    gap: 12px;
    transition: all 0.28s cubic-bezier(0.2,0,0,1);
  }

  .feature:hover {
    border: 1px solid rgba(var(--text-color-rgba), 0.4);
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    transform: translateY(-4px);
  }

  .feature_icon {
    min-width: 36px;
    height: 36px;

    display: flex;
    align-items: center;
    justify-content: center;

    border-radius: 300px;
  }

  .feature_text {
    display: flex;
    flex-direction: column;
    gap: 4px;
  }

  .feature_title {
    font-size: 1.1em;
    font-weight: 600;
    color: var(--text-color);
    margin: 0;
  }

  .feature_description {
    font-size: 0.95em;
    line-height: 1.2em;
    font-weight: 400;
    color: var(--text-color);
  }

  @media (max-width: 900px) {
    .features {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media (max-width: 600px) {
    .features {
      grid-template-columns: repeat(1, 1fr);
    }
  }
</style>
