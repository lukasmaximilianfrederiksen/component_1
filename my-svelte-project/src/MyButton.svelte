<script>
  export let type;
</script>

<button class={type}>
  <slot />
</button>

<style>
  button {
    border: none;
    border-radius: 8px;
    color: white;
    width: 120px;
    height: 40px;
    background: var(--default-color);
    transition: all 0.3s;
    cursor: pointer;
    font-family: "Roboto", sans-serif;
    font-size: 1rem;
  }

  .primary {
    background: var(--Primary-color);
  }

  .primary:hover {
    background-color: hsla(251, 85%, 75%, 1);
  }

  .secondary {
    background: var(--Secondary-color);
  }

  .secondary:hover {
    background: hsla(315, 70%, 74%, 1);
  }

  .accent {
    background: var(--Accent-color);
  }

  .accent:hover {
    background: hsla(173, 48%, 80%, 1);
  }

  .ghost {
    background: var(--Ghost-bg-color);
    color: var(--Ghost-color);
  }

  .ghost:hover {
    color: hsla(220, 13%, 68%, 1);
  }

  .link {
    background: var(--Ghost-bg-color);
    color: var(--Link-color);
  }

  .link:hover {
    color: hsla(251, 85%, 79%, 1);
  }

  .neutral:hover {
    background: hsla(0, 0%, 39%, 1);
  }
</style>
