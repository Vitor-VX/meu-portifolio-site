<script lang="ts">
import Hero from './components/Hero.svelte';
import About from './components/About.svelte';
import Skills from './components/Skills.svelte';
import Projects from './components/Projects.svelte';
import Contact from './components/Contact.svelte';
</script>

<main>
  <Hero />
  <About />
  <Skills />
  <Projects />
  <Contact />
</main>

<style>
  main {
    width: 100%;
    min-height: 100vh;
    background-color: var(--color-background);
  }
</style>