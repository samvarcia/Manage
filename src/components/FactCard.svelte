<script>
  export let title;
  export let text;
</script>

<style>
  .FactCard-content p {
    color: var(--main-gray);
    width: 450px;
  }
  @media screen and (max-width: 768px) {
    .FactCard-content li h3 {
      color: var(--main-orange);
    }
    .FactCard-content p {
      font-size: 13px;
      width: 300px;
    }
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
