<script>
  import Badge from "./Badge.svelte";
  import MyButton from "./MyButton.svelte";
</script>

<div class="container">
  <div class="card">
    <div class="card-header">
      <img src="./billeder/sko.jpg" alt="rover" />
    </div>
    <div class="card-body">
      <h4>Shoes!</h4>

      <Badge type="secondary" title="NEW" />
    </div>
    <p>If a dog chews shoes whose shoes does he choose?</p>
    <div class="badgeContainer">
      <div class="single_badge">
        <Badge type="border" title="Fashion" />
      </div>
      <div class="single_badge">
        <Badge type="border" title="Products" />
      </div>
    </div>

    <div class="buttoncontainer">
      <MyButton type="primary">Buy Now</MyButton>
    </div>
  </div>
</div>

<style>
  .container {
    display: flex;
    width: auto;
    justify-content: space-evenly;
    flex-wrap: wrap;
  }
  .card {
    margin: 10px;
    background-color: #fff;
    border-radius: 10px;
    box-shadow: 0 2px 20px rgba(0, 0, 0, 0.2);
    overflow: hidden;
    width: 300px;
    height: 400px;
  }
  .card-header img {
    width: 100%;
    height: 200px;
    object-fit: cover;
  }
  .card-body {
    display: flex;
    flex-direction: row;
    align-items: flex-start;

    align-items: center;
    height: 30px;
  }
  .single_badge {
    padding: 5px;
  }
  h4 {
    color: black;
    padding-left: 10px;
    padding-right: 10px;
  }

  p {
    color: black;
    padding: 10px;
  }

  .badgeContainer {
    display: flex;
    flex-direction: row;
    padding-left: 5px;
    padding-right: 10px;
  }

  .buttoncontainer {
    display: flex;
    justify-content: flex-end;
    padding-left: 10px;
    padding-right: 20px;
    padding-top: 5px;
    padding-bottom: 20px;
  }
  .tag {
    background: #cccccc;
    border-radius: 50px;
    font-size: 12px;
    margin: 0;
    color: rgb(0, 0, 0);
    padding: 2px 10px;
    text-transform: uppercase;
    cursor: pointer;
  }
</style>
