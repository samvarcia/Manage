<script>
  export let image;
  export let UserName;
  export let UserText;
</script>

<style>
  .UserCard-content img {
    border-radius: 50%;
    width: 100px;
  }
  .UserCard-content p {
    width: 300px;
    color: var(--main-gray);
  }
  .UserCard-card {
    text-align: center;
    margin: 10px;
  }
</style>

<div class="UserCard">
  <div class="UserCard-container">
    <div class="UserCard-content">
      <div class="UserCard-card">
        <img src={image} alt="Users" />
        <div>
          <h1>{UserName}</h1>
          <p>{UserText}</p>
        </div>
      </div>
    </div>
  </div>
</div>
