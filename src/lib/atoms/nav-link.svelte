<script>
  export let LinkRoute, LinkText, NavIcons, NavIconsAlt;
</script>

<a href={LinkRoute}
  ><img src={NavIcons} alt="NavIconsAlt" />
  <p>{LinkText}</p>
</a>

<style>
  a {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    text-decoration: none;
    font-family: var(--secondary-font-family);
    font-size: 0.8rem;
    font-weight: 500;
    color: var(--primary-font-color);
    aspect-ratio: 5/4;
  }

  img {
    width: 100%;
    max-width: 3rem;
  }

  p {
    width: 80%;
    font-size: clamp(.8rem, 1vw, 1rem);
}
</style>
