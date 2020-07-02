<script>
  import Button from "./ButtonWhite.svelte";
</script>

<style>
  .Banner {
    margin-top: 40px;
  }
  .Banner-container {
    background-color: var(--main-orange);
    padding: var(--container);
  }
  .Banner-content {
    display: flex;
    align-items: center;
    justify-content: space-between;
    color: #fff;
    flex-wrap: wrap;
  }
</style>

<div class="Banner">
  <div class="Banner-container">
    <div class="Banner-content">
      <div class="Banner-title">
        <h1>
          Simplify how your team
          <br />
          works today.
        </h1>
      </div>
      <Button />
    </div>
  </div>
</div>
