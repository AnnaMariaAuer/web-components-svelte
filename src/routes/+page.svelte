<script lang="ts">
  import "../index.css";
  import Hero from "$lib/hero/Hero.svelte";
  import Button from "../lib/button/Button.svelte";
  import heroImage from "$lib/assets/anna2.jpeg";
</script>

<h1>Welcome to your library project</h1>
<p>
  Create your package using @sveltejs/package and preview/showcase your work
  with SvelteKit
</p>
<p>
  Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the
  documentation
</p>
<Button label="Test" variant="outlined" onClick={() => console.log("test")} />

<Hero
  title="Webdesign"
  subtitle="Klar. Flexibel. Für Dich."
  imageUrl={heroImage}
  classBg="hero-bg"
  cta={{ label: "Sag Hallo 👋🏼", href: "some-url" }}
/>
