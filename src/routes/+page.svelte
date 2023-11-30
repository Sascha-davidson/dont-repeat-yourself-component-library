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
    display: grid;
    grid-template-columns: 1.25fr 1.25fr 1fr 1fr;
    grid-template-rows: 1.5fr 1.5fr 2fr;
    height: 100vh;
    width: 100%;
    gap: 2rem;
  }

  section,
  a {
    border-radius: 25px;
    box-shadow: var(--box-shadow);
    padding: 4vh 3vw;
  }

  a:nth-of-type(1) a {
    background-color: #e7fff7;
    overflow: hidden;
  }

  /* tournaments new */
  a:nth-of-type(1) {
    grid-area: 1 / 1 / 2 / 3;
    background-color: #e7fff7;
  }

  /* teams new */
  a:nth-of-type(2) {
    grid-area: 2 / 1 / 2 / 2;
    background-color: #e7fff7;
  }

  /* players new */
  a:nth-of-type(3) {
    grid-area: 2 / 2 / 2 / 3;
    background-color: #e7fff7;
  }

  /* Completed Tournaments */
  a:nth-of-type(4) {
    grid-area: 1 / 3 / 3 / 5;
    background-color: #fff;
  }

  /* Current Tournament */
  a:nth-of-type(5) {
    grid-area: 3 / 1 / 3 / 4;
    background-color: #d6dcff;
  }

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    box-shadow: var(--box-shadow);
    border-radius: 25px;
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
