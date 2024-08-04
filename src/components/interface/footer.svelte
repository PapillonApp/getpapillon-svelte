<script>
    import { Github, Instagram, MessagesSquare, Twitter, Linkedin } from "lucide-svelte";

</script>
<div class="footer">
  <div class="width">
    <p class="footer-text">
      © 2024, <a href="https://github.com/PapillonApp">PapillonApp</a> et leurs contributeurs associés.<br/>
      Papillon n'est affilié à aucune entreprise ou organisation.
    </p>

    <div class="nav-social">
      <a href="https://twitter.com/thepapillonapp" target="_blank" rel="noopener noreferrer" aria-label="Twitter">
        <Twitter size="24" />
      </a>
      <a href="https://github.com/PapillonApp" target="_blank" rel="noopener noreferrer" aria-label="Github">
        <Github size="24" />
      </a>
      <a href="https://instagram.com/thepapillonapp" target="_blank" rel="noopener noreferrer" aria-label="Instagram">
        <Instagram size="24" />
      </a>
      <a href="https://discord.gg/ywkBZx2jFB" target="_blank" rel="noopener noreferrer" aria-label="Discord">
        <MessagesSquare size="24" />
      </a>
      <a href="https://www.linkedin.com/company/getpapillonapp/" target="_blank" rel="noopener noreferrer" aria-label="Linkedin">
        <Linkedin size="24" strokeWidth="1.75" />
      </a>
    </div>
  </div>
</div>

<style>
  .footer {
    background-color: var(--background-over-100);
    color: #fff;
    padding: 20px 0;
  }

  .footer .width {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .footer a {
    color: #fff;
    text-decoration: none;
  }

  .footer a:hover {
    text-decoration: underline;
  }

  .footer-text {
    text-align: flex-start;
    opacity: 0.6;
    font-size: 0.8em;
  }

  .nav-social {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 16px;
  }

  .nav-social a {
    color: #fff;
    opacity: 0.6;
  }

  .nav-social a:hover {
    opacity: 1;
  }
</style>