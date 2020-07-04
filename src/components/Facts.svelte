<script>
  import FactCard from "./FactCard.svelte";
</script>

<style>
  .Facts-container {
    padding: var(--container);
  }
  .Facts-content {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }

  @media screen and (max-width: 768px) {
    .Facts-container {
      padding: 0;
      text-align: center;
    }
    .Facts-content {
      justify-content: center;
    }
    ol {
      padding: 0;
    }
  }
</style>

<div class="Facts">
  <div class="Facts-container">
    <div class="Facts-content">
      <div class="Facts-main">
        <h1>
          What's different about
          <br />
          Manage?
        </h1>
        <p>
          Manage provides all the functionality your
          <br />
          team needs, without the complexity. Our
          <br />
          software is tailor-made for modern digital
          <br />
          product teams.
        </p>
      </div>
      <div class="Facts-list">
        <ol>
          <FactCard
            title="Track company-wide progress"
            text="See how your day-to-day tasks fit into the wider vision. Go
            from tracking progress at the milestone level all the way done to
            the smallest of details. Nver lose sight of the bigger picture
            again." />
          <FactCard
            title="Advanced built-in reports"
            text="Set internal delivery estimates and track progress toward
            company goals. Our customisable dashboard helps you build out the
            reports you need to keep key stakeholders informed." />
          <FactCard
            title="Everything you need in one place"
            text="Stop jumping from one service to another to communicate, store
            files, track tasks and share documents. Manage offers an all-in-one
            team productivity solution." />
        </ol>
      </div>
    </div>
  </div>
</div>
