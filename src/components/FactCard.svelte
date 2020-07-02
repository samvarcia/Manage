<script>
  export let title;
  export let text;
</script>

<style>
  .FactCard-content p {
    color: var(--main-gray);
    width: 450px;
  }
</style>

<div class="FactCard">
  <div class="FactCard-container">
    <div class="FactCard-content">
      <li>
        <h3>{title}</h3>
        <p>{text}</p>
      </li>
    </div>
  </div>
</div>
