<script lang="ts">
  import Icon from '@iconify/svelte';
  
  const currentYear = new Date().getFullYear();
</script>

<section id="contact" class="contact">
  <div class="container">
    <h2>Contato</h2>
    <div class="social-links">
      <a href="https://wa.me/556993161840" target="_blank" rel="noopener noreferrer" class="social-link">
        <Icon icon="logos:whatsapp" width="24" />
      </a>
      <a href="https://github.com/vitor-vx" target="_blank" rel="noopener noreferrer" class="social-link">
        <Icon icon="mdi:github" width="24" />
      </a>
      <a href="https://www.threads.net/@if_vitor" target="_blank" rel="noopener noreferrer" class="social-link">
        <Icon icon="ri:threads-fill" width="24" />
      </a>
      <a href="https://instagram.com/if_vitor" target="_blank" rel="noopener noreferrer" class="social-link">
        <Icon icon="mdi:instagram" width="24" />
      </a>
    </div>
    <footer class="footer">
      <p>&copy; {currentYear} - Todos os direitos reservados</p>
    </footer>
  </div>
</section>

<style>
  .contact {
    text-align: center;
    background: rgba(255, 255, 255, 0.02);
  }

  .social-links {
    display: flex;
    justify-content: center;
    gap: 2rem;
    flex-wrap: wrap;
    margin-bottom: 3rem;
  }

  .social-link {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 3rem;
    height: 3rem;
    background: rgba(255, 255, 255, 0.05);
    border-radius: 50%;
    text-decoration: none;
    color: var(--color-text);
    transition: all 0.3s ease;
  }

  .social-link:hover {
    background: rgba(255, 255, 255, 0.1);
    transform: translateY(-2px);
    color: var(--color-text);
  }

  .footer {
    padding-top: 2rem;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
    color: var(--color-text-muted);
    font-size: 0.9rem;
  }

  @media (max-width: 768px) {
    .social-links {
      gap: 1rem;
    }
  }
</style>