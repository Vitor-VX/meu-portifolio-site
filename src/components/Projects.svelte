<script lang="ts">
  import Icon from "@iconify/svelte";
  import casinoImage from "../assets/img_casino_2.jpg";
  import minesImage from "../assets/img_mines.png";
</script>

<section id="projects" class="projects">
  <div class="container">
    <h2>Projetos</h2>

    <div class="project">
      <h3>Cassino App</h3>
      <div class="project-content">
        <div class="project-image">
          <div class="image-placeholder">
            <img src={casinoImage} alt="Imagem do cassino" />
          </div>
        </div>
        <div class="project-info">
          <p>
            Um aplicativo moderno de cassino desenvolvido com Jetpack Compose,
            oferecendo uma experiência de usuário fluida e envolvente.
          </p>
          <div class="tech-stack">
            <span class="tech">
              <Icon icon="devicon:kotlin" width="20" />
              Kotlin
            </span>
            <span class="tech">
              <Icon icon="simple-icons:jetpackcompose" width="20" />
              Jetpack Compose
            </span>
          </div>
        </div>
      </div>
    </div>

    <div class="project">
      <h3>Jogo Mobile</h3>
      <div class="project-content">
        <div class="project-image">
          <div class="image-placeholder">
            <img src={minesImage} alt="Jogo do Mines" />
          </div>
        </div>
        <div class="project-info">
          <p>
            Um jogo do Mines desenvolvido com as mais recentes tecnologias
            Android. <strong>Podendo ser adaptado para jogos de azar.</strong>
          </p>
          <div class="tech-stack">
            <span class="tech">
              <Icon icon="devicon:kotlin" width="20" />
              Kotlin
            </span>
            <span class="tech">
              <Icon icon="simple-icons:jetpackcompose" width="20" />
              Jetpack Compose
            </span>
          </div>
        </div>
      </div>
    </div>

    <div class="project">
      <h3>WhatsApp Bot com IA</h3>
      <div class="project-content">
        <div class="project-info">
          <p>
            Bot inteligente para WhatsApp integrado com IA para automação de
            atendimento ao cliente.
          </p>
          <p><em>Acesse com uma conta temporária: contateste@gmail.com/12345@a</em></p>
          <div class="tech-stack">
            <span class="tech">
              <Icon icon="logos:nodejs" width="20" />
              Node.js
            </span>
            <span class="tech">
              <Icon icon="logos:typescript-icon" width="20" />
              TypeScript
            </span>
            <span class="tech">
              <Icon icon="logos:openai-icon" width="20" />
              OpenAI
            </span>
          </div>
          <a
            href="https://vxchatbot.site/login"
            target="_blank"
            rel="noopener noreferrer"
            class="demo-link"
          >
            <Icon icon="mdi:link-variant" width="20" />
            Acessar Demonstração (conta temporária)
          </a>
        </div>
      </div>
    </div>

  </div>
</section>

<style>
  .projects {
    background: rgba(255, 255, 255, 0.01);
  }

  .project {
    background: rgba(255, 255, 255, 0.03);
    border-radius: 1rem;
    padding: 2rem;
    margin-bottom: 3rem;
  }

  .project:last-child {
    margin-bottom: 0;
  }

  h3 {
    font-family: "Poppins", sans-serif;
    font-size: 1.5rem;
    margin-bottom: 1rem;
    background: var(--gradient-primary);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
    display: inline-block;
  }

  .project-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
  }

  .project-image {
    width: 100%;
    aspect-ratio: 16/9;
    border-radius: 0.5rem;
    overflow: hidden;
  }

  .project-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  .image-placeholder {
    width: 100%;
    height: 100%;
    background: rgba(255, 255, 255, 0.05);
    display: flex;
    align-items: center;
    justify-content: center;
    color: var(--color-text-muted);
  }

  .project-info p {
    color: var(--color-text-muted);
    margin-bottom: 1.5rem;
    line-height: 1.6;
  }

  .tech-stack {
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
    margin-bottom: 1.5rem;
  }

  .tech {
    background: rgba(255, 255, 255, 0.1);
    padding: 0.5rem 1rem;
    border-radius: 2rem;
    font-size: 0.9rem;
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .demo-link {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    padding: 0.75rem 1.5rem;
    background: var(--gradient-primary);
    border-radius: 2rem;
    color: white;
    text-decoration: none;
    font-weight: 500;
    transition: all 0.3s ease;
  }

  .demo-link:hover {
    transform: translateY(-2px);
    opacity: 0.9;
  }

  @media (max-width: 768px) {
    .project {
      padding: 1.5rem;
    }

    .project-content {
      grid-template-columns: 1fr;
    }
  }
</style>
