<script>
</script>

<main>
  <a href="/CreateTournament">
    <h2>Create Tournament</h2>
    <p class="subtitle-medium">Create your tournament</p>
  </a>
  <a href="/CreateTeam">
    <h3 class="subtitle-large">Create Team</h3>
    <p class="subtitle-small">Create your team</p>
  </a>
  <a href="/CreatePlayer">
    <h3 class="subtitle-large">Create Player</h3>
    <p class="subtitle-small">Create your player</p>
  </a>
  <a href="/CompletedTournaments">
    <h2>Completed Tournaments</h2>
    <p class="subtitle-medium">View the completed tournaments</p>
  </a>
  <a href="CurrentTournament">
    <h2>Current Tournament</h2>
    <p class="subtitle-medium">Check the current tournament</p>
  </a>
  <img src="../images/frisbee-3.png" alt="frisbee" />
</main>

<style>
  main {
    grid-template-columns: 1.25fr 1.25fr 1fr 1fr;
    grid-template-areas:
      "CreateTournament CreateTournament CompletedTournaments CompletedTournaments"
      "CreateTeam CreatePlayer CompletedTournaments CompletedTournaments"
      "CurrentTournament CurrentTournament CurrentTournament Image";
  }

  a {
    border-radius: 25px;
    box-shadow: var(--box-shadow);
    padding: 4vh 3vw;
  }

  a:nth-of-type(1) {
    grid-area: CreateTournament;
    background-color: #e7fff7;
  }

  a:nth-of-type(2) {
    grid-area: CreateTeam;
    background-color: #e7fff7;
  }

  a:nth-of-type(3) {
    grid-area: CreatePlayer;
    background-color: #e7fff7;
  }

  a:nth-of-type(4) {
    grid-area: CompletedTournaments;
    background-color: #fff;
  }

  a:nth-of-type(5) {
    grid-area: CurrentTournament;
    background-color: #d6dcff;
  }

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    box-shadow: var(--box-shadow);
    border-radius: 25px;
    grid-area: Image;

  }

  /*RESPONSIVE KLOPT NOG NIET HELEMAAL*/

  /* @media only screen and (max-width: 580px){
        main{
            display: grid;
            grid-template-columns: 1fr;
            height: fit-content;
            width: 100vw;
            gap: 2rem;
        }

        section:nth-of-type(1){
            grid-area: 1 / 1;
        }

        section:nth-of-type(2){
            grid-area: 2 / 1;
        }

        section:nth-of-type(3){
            grid-area: 3 / 1;
        }
        
        section:nth-of-type(4){
            grid-area: 4 / 1;
        }
    } */
</style>
