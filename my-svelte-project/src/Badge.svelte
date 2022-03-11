<script>
  export let type;
  export let title;
</script>

<div class={type}>
  <span>{title}</span>
</div>

<style>
  div {
    text-align: center;
    border: none;
    border-radius: 14px;
    color: white;
    width: min-content;
    height: 22px;
    background: var(--default-color);
    transition: all 0.3s;
    cursor: pointer;
    padding-top: 5px;
    padding-bottom: 3px;
    padding-left: 10px;
    padding-right: 10px;
  }

  span {
    padding-top: 2px;
  }

  .border {
    background: none;
    border: solid 2px black;
    color: black;
    width: min-content;
  }

  .neutral:hover {
    background: hsla(0, 0%, 49%, 1);
  }
  .primary {
    background: var(--Primary-color);
  }

  .primary:hover {
    background: hsla(251, 85%, 75%, 1);
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
  }
</style>
