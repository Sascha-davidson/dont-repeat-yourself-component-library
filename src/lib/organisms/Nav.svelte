<script>
  import NavLink from "$lib/atoms/nav-link.svelte"
</script>

<div class="nav-container">
  <nav>
    <ul>
      <li>
        <NavLink LinkRoute="/" LinkText="Home" NavIcons="/images/home-icon.svg" NavIconsAls="" />
      </li>
      <li>
        <NavLink LinkRoute="/players" LinkText="All Players" NavIcons="/images/all-players-icon.svg" NavIconsAls="" />
      </li>
      <li>
        <NavLink LinkRoute="/teams" LinkText="All Teams" NavIcons="/images/all-teams-icon.svg" NavIconsAls="" />
      </li>
      <li>
        <NavLink LinkRoute="/tournaments" LinkText="All Tournaments" NavIcons="/images/all-tournaments-icon.svg" NavIconsAls="" />
      </li>
      <li>
        <NavLink LinkRoute="/players" LinkText="Current Tournament" NavIcons="/images/current-tournament-icon.svg" NavIconsAls="" />
      </li>
    </ul>
  </nav>
</div>

<style>
  .nav-container {
    height: 100vh;
    padding: 0.8rem;
  }

  nav {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: var(--element-background-color);
    height: 100%;
    min-width: 90px;
    border-radius: 10px;
    box-shadow: var(--box-shadow);
  }

  ul {
    display: flex;
    flex-direction: column;
    gap: 1em;
    list-style: none;
    width: 100%;
  }


</style>
