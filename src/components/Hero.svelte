<script>
  import Button from "./Button.svelte";
  let graph = "images/illustration-intro.svg";
</script>

<style>
  .Hero-container {
    padding: var(--container);
    font-family: "Be Vietnam", sans-serif;
  }
  .Hero-content {
    display: flex;
    flex-wrap: wrap-reverse;
    justify-content: space-between;
    align-items: center;
  }
  .Hero-copy h1 {
    font-size: 55px;
  }
  .Hero-copy p {
    color: var(--main-gray);
    line-height: 28px;
  }
  @media screen and (max-width: 768px) {
    .Hero-container {
      padding: 0;
    }
  }
</style>

<div class="Hero">
  <div class="Hero-container">
    <div class="Hero-content">
      <div class="Hero-copy">
        <h1>
          Bring everyone
          <br />
          together to build
          <br />
          better products.
        </h1>
        <p>
          Manage makes it simple for software teams
          <br />
          to plan day-to-day tasks while keeping the
          <br />
          larger team goals in view.
        </p>
        <Button />
      </div>
      <div class="Hero-graph">
        <img src={graph} alt="Stats" />
      </div>
    </div>
  </div>
</div>
