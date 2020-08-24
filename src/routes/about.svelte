<script>
  import { fade } from "svelte/transition";

  const quote = `So, there's these, like, yinger and yangerons, and they spin in this projected pattern which intersects fourth-dimensionally. But it isn't a measurable function. It's got a whoosh, whoom, whoooooooooh!`;

  const ahem = `Anyways, here's the boring technical part. ZzZzZz...`;

  const creator = `Hey, I'm PraZ! I'm a web developer and also a Zoe one trick. I made this small cute bot to help one of my favourite community however I could. If you encounter any issue, or want to talk about the bot or any JavaScript code, feel free to message me on discord @ PraZ#4184.`;

  const github = `Here is a link to my GitHub repo. You will find all the technical informations needed to run your own ZoeBot. If you encounter any problem, open an issue or fork the repo and fill a PR with a fix!`;

  const website = `This website is a desperate attempt to force my creator to use Svelte. Uh, I don't think he's enjoying it... :(`;
</script>

<style>
  h1 {
    margin: 0.5em 0 0.5em 0;
    border-bottom: solid 2px #0b9d73;
  }

  quote {
    font-size: 1.3rem;
    font-style: italic;
  }

  p {
    font-size: 1.3rem;
  }

  a {
    font-size: 1.4em;
    text-align: center;
  }

  .link-container {
    text-align: center;

    font-size: 1.1rem;
  }

  .link-container :focus {
    color: #0b9d73;
  }

  .link-container :hover {
    color: #0b9d73;
  }
</style>

<svelte:head>
  <title>ZoeBot4 | About</title>
</svelte:head>

<div in:fade={{ duration: 750 }}>
  <quote>{quote}</quote>
  <p style="text-align: right;">{ahem}</p>

  <h1>{`A word from my creator...`}</h1>
  <p>{creator}</p>

  <h1>{`You want the magic code and nerd stuff?`}</h1>
  <p>{github}</p>
  <div class="link-container">
    <a alt="ZoeBot4 github repo" href="https://github.com/prazdevs/zoe-bot-4">
      To the GitHub!
    </a>
  </div>

  <h1>{`About this website...`}</h1>
  <p>{website}</p>
</div>
