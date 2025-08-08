<script lang="ts">
  import "./button.scss";

  export let label: string;
  export let onClick: () => void;
  export let variant: "primary" | "outlined" | "text" = "primary";
</script>

<button onclick={onClick} class={`button-${variant}`}>
  {label}
</button>
