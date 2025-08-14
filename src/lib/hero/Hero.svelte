<script lang="ts">
  import "./hero.scss";
  import Button from "$lib/button/Button.svelte";

  interface Props {
    title: string;
    subtitle?: string;
    imageUrl: string;
    classBg?: string;
    classSubtitle?: string;
    cta: {
      label: string;
      onClick?: () => void;
      href?: string;
    };
  }

  let { title, subtitle, imageUrl, classBg, classSubtitle, cta }: Props =
    $props();
</script>

<div class={classBg}>
  <div class="hero-text">
    <h1>
      {title}
      {#if subtitle}
        <div class={classSubtitle}>{subtitle}</div>
      {/if}
    </h1>
    <Button {...cta} />
  </div>
  <div class="hero">
    <img src={imageUrl} alt="" />
  </div>
</div>
