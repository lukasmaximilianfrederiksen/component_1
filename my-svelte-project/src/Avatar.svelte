<script>
  export let initial;
  export let size;
  export let mode;
</script>

<div class="container">
  <div class={size}>
    <div class:indikator={mode === "indikator"} />
    <span>{initial}</span>
  </div>
</div>

<style>
  .container {
    position: relative;
  }

  .mainCircle {
    display: flex;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background: var(--default-color);
    justify-content: center;
    align-items: center;
  }

  .mainCircleMedium {
    display: flex;
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background: var(--default-color);
    justify-content: center;
    align-items: center;
  }

  .mainCircleSmall {
    display: flex;
    width: 30px;
    height: 30px;
    border-radius: 50%;
    background: var(--default-color);
    justify-content: center;
    align-items: center;
  }

  .mainCircleExtraSmall {
    display: flex;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background: var(--default-color);
    justify-content: center;
    align-items: center;
  }

  .mainCircleSmall span {
    font-size: small;
  }

  .indikator {
    width: 20%;
    height: 20%;
    position: absolute;
    top: 2%;
    right: 0%;
    border-radius: 50%;
    border: solid 2px white;
    background-color: rgb(24, 250, 3);
  }
</style>
