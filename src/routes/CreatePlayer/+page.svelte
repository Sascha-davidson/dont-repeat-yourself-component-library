<script>
  import Form from "$lib/organisms/form.svelte";
  import Button from "$lib/atoms/button.svelte";
  import LinkButton from "$lib/atoms/link-button.svelte";
</script>

<main>
  <h2 id="title">Create Player</h2>
  <h3 class="CreatePlayer">who are you adding </h3>
  <h3 class="AddPlayer">Add player to team</h3>
  <Form FormID="FormID" Method="get" Action="/AllPlayers" />
  <Button ButtonType="submit" ButtonText="Save" FormID="FormID" />
  <!-- <LinkButton Routing="/" LinkText="Next Page" /> -->
  <p class="other">other data</p>
</main>

<style>
  main {
    grid-template-columns: 1fr 1fr;
    grid-template-areas:
      "Title Title"
      "CreatePlayer AddPlayer"
      "form other"
      "button button";
  }

  h2 {
    grid-area: Title;
  }

  p {
    padding: 0 5px;
  }

  .CreatePlayer {
    grid-area: CreatePlayer;
  }

  .AddPlayer {
    grid-area: AddPlayer;
  }

  .other {
    grid-area: other;
  }
</style>
