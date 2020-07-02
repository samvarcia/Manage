<script>
  import Button from "./Button.svelte";
  import UserCard from "./UserCard.svelte";

  let AvatarElon = "images/elon-musk.jpg";
  let AvatarJeff = "images/jeff-bezos.jpg";
  let AvatarMark = "images/mark-zuck.jpeg";
</script>

<style>
  .Users-content {
    text-align: center;
  }
  .Users-cards {
    padding: 50px;
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    justify-content: space-around;
  }
</style>

<div class="Users">
  <div class="Users-container">
    <div class="Users-content">
      <div class="Users-title">
        <h1>What they've said</h1>
      </div>
      <div class="Users-cards">
        <UserCard
          image={AvatarElon}
          UserName="Elon Musk"
          UserText="Manage has supercharged our team's workflow. The ability to
          maintain visibility on larger milestones at all times keeps everyone
          motivated." />
        <UserCard
          image={AvatarJeff}
          UserName="Jeff Bezos"
          UserText="We have been able to cancel so many other subscriptions
          since using Manage. There is no more cross-channel confusion and
          everyone is much more focused." />
        <UserCard
          image={AvatarMark}
          UserName="Mark Zuckerberg"
          UserText="Manage allows us to provide structure and process. It keeps
          us organized and focused. I can't stop recommending them to everyone i
          talk to!" />
      </div>
      <Button class="boton" />
    </div>
  </div>
</div>
