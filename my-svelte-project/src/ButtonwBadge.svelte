<script>
  import Badge from "./Badge.svelte";
  import MyButton from "./MyButton.svelte";
</script>

<div class="container">
  <div class="knap"><MyButton type="neutral">Inbox</MyButton></div>
  <div class="tal">
    <Badge type="secondary" title="99+" />
  </div>
</div>

<style>
  .container {
    position: relative;
    width: min-content;
  }

  .container .tal {
    position: absolute;
    top: -20px;
    right: -30px;
    padding: 5px 10px;
    border-radius: 50%;

    color: white;
  }
</style>
