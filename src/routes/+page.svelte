<script>
    import Form from "$lib/organisms/form.svelte";
    import Button from "$lib/atoms/button.svelte";
    import LinkButton from "$lib/atoms/link-button.svelte";
  </script>
  
  <div>
    <main>
      <h2 id="title">Create Player</h2>
      <p class="CreatePlayer">Create a player</p>
      <p class="AddPlayer">Add player to team</p>
      <Form FormID="FormID" Method="get" Action="/AllPlayers"/>
      <Button ButtonType="submit" ButtonText="Save" FormID="FormID"/>
      <!-- <LinkButton Routing="/" LinkText="Next Page" /> -->
      <p class="other">other data</p>
    </main>
  
    <!-- <Nav /> -->
  </div>
  
  <style>
    div {
      display: flex;
      height: 100%;
    }
  
    main {
      height: 100%;
      width: 100%;
      display: grid;
      grid-template-columns: 1fr 1fr;
      grid-template-rows: auto auto 1fr auto;
      /* column-gap: 2rem;
      row-gap: 0; */
      gap: 2rem;
      padding: 4rem 4%;
      grid-template-areas:
        "Title Title"
        "CreatePlayer AddPlayer"
        "form other"
        "button button";
    }
  
    h2 {
      grid-area: Title;
      padding: 0 5px;
    }
  
    p{
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
  