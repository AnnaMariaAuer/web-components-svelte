<script lang="ts">
  import "./button.scss";

  interface ButtonProps {
    label: string;
    variant?: "primary" | "outlined" | "text";
    onClick?: () => void;
    href?: string;
  }

  let { label, variant = "primary", onClick, href }: ButtonProps = $props();
</script>

{#if href}
  <a {href} class={`link-${variant}`}>{label}</a>
{:else}
  <button onclick={onClick} class={`button-${variant}`}>
    {label}
  </button>
{/if}
