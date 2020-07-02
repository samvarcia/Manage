<script>
  import Button from "./Button.svelte";
  let Logo = "images/logo.svg";
</script>

<style>
  .Header {
    font-family: "Be Vietnam", sans-serif;

    width: 100%;
  }
  .Header-container {
    padding: var(--container);
  }
  .Header-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  ul {
    display: flex;
    list-style: none;
  }
  .Header b {
    padding: 0.5rem;
    font-size: 16px;
    cursor: pointer;
  }
  .Header b:hover {
    color: #9d9ea2;
  }
  .Header button {
    background-color: hsl(12, 88%, 59%);
    color: #fff;
    width: 120px;
    height: 40px;
    font-size: 12px;
    border-radius: 100px;
    font-weight: bold;
    cursor: pointer;
  }
  .Header button:hover {
    background-color: #f98e75;
  }
</style>

<div class="Header">
  <div class="Header-container">
    <div class="Header-content">
      <div class="Header-logo">
        <img src={Logo} alt="" />
      </div>
      <div class="Header-nav">
        <ul>
          <li>
            <b>Pricing</b>
          </li>
          <li>
            <b>Product</b>
          </li>
          <li>
            <b>About Us</b>
          </li>
          <li>
            <b>Careers</b>
          </li>
          <li>
            <b>Community</b>
          </li>
        </ul>
      </div>
      <Button />
    </div>
  </div>
</div>
