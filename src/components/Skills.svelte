<script lang="ts">
  import Icon from "@iconify/svelte";

  const skills = [
    { name: "Kotlin", icon: "devicon-plain:kotlin-wordmark" },
    { name: "Jetpack Compose", icon: "mdi:android" },
    { name: "Java", icon: "devicon:java" },
    { name: "JavaScript", icon: "devicon:javascript" },
    { name: "Node.js", icon: "devicon:nodejs" },
    { name: "Svelte", icon: "devicon:svelte" },
    { name: "HTML5", icon: "devicon:html5" },
    { name: "CSS3", icon: "devicon:css3" },
    { name: "TypeScript", icon: "devicon:typescript" },
    { name: "Browser Automation", icon: "mdi:robot-outline" },
    { name: "APIs Robustas", icon: "mdi:api" },
    { name: "Ktor", icon: "logos:ktor" },
  ];
</script>

<section class="skills">
  <div class="container">
    <h2>Skills</h2>
    <div class="container-skills">
      {#each skills as skill (skill.name)}
        <Icon icon={skill.icon} width="200" height="72" />
      {/each}
    </div>
  </div>
</section>

<style>
  .skills {
    padding: 2rem;
  }

  h2 {
    font-family: "Poppins", sans-serif;
    font-size: 2.5rem;
    color: #eee;
    background: linear-gradient(to right, #8a2be2, #40e0d0);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 2.5rem;
  }

  .container {
    max-width: 1100px;
    margin: 0 auto;
    text-align: center;
  }

  .container-skills {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1.5rem;
  }
</style>