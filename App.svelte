<script>
  import Crossword from "svelte-crossword";
  import dataInput from "./data/mama.json";

</script>

<article>
  <div class="intro">
    <p>
      Birthday Puzzle for Mama :)
    </p>
  </div>

  <section id="slots">
    <Crossword data="{dataInput}">
      <div slot="message">
        <h3>Yay! Happy Birthday!</h3>
        <img
          alt="celebration"
          src="mama.jpg" width="100%"/>
      </div>
    </Crossword>
  </section>
</article>

<style>
  article {
    max-width: 960px;
    margin: 0 auto;
    padding: 1em;
    font-family: sans-serif;
  }
  .intro {
    text-align: left;
    max-width: 760px;
    font-size: 1.5em;
  }
  section {
    max-width: 960px;
    margin: 5em 0;
  }

  .info {
    max-width: 640px;
    margin: 1em 0;
    text-align: left;
    font-size: 1.125em;
  }
  .info a {
    margin-right: 0.25em;
  }
  h1 {
    font-size: 1.5em;
  }
  h2 {
    font-size: 1.5em;
    padding-top: 1em;
  }
  p {
    margin: 1em auto;
    text-align: center;
  }

  #themes {
    padding: 1em;
  }

  #themes.dark {
    background: #1a1a1a;
    color: #fff;
  }
  code {
    font-size: 0.85em;
    background-color: #efefef;
    padding: 0 0.25em;
  }

  button {
    cursor: pointer;
  }
</style>
