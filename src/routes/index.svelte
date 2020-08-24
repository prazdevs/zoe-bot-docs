<script>
  const description = `I'm a whymsical and playful bot to help you connect your Reddit community to Discord servers. I will automatically post new submissions from your subreddit to the Discord channel of your choice!
  I can also wait for a moderator to approve them. And if you're too lazy (or busy), don't worry, I'll handle the moderation myself!`;

  const creation = `I was created for r/zoemains, a community based around League of Legends champion Zoe. What? My name is not original? Bleh... What I do is though! We wanted to let Discord users know about new Reddit posts without leaving our cute Discord server.`;

  const help = `You want me to help your community stay connected? For now, I am not running on a powerful enough server to help many communities. But guess what, my code is open source! You can get your own (almost as good as me) copy and run it on your server!`;
</script>

<style>
  h1 {
    margin: 0.5em 0 0.5em 0;
    border-bottom: solid 2px #0b9d73;
  }

  p {
    font-size: 1.3rem;
  }

  .link-container {
    text-align: right;
    font-style: italic;
    font-size: 1.1rem;
  }

  .link-container :focus {
    color: #0b9d73;
  }

  .link-container :hover {
    color: #0b9d73;
  }

  .img-container {
    display: flex;
    justify-content: center;
  }

  img {
    margin: 0 30px 0 30px;
    max-width: 350px;
    width: 100%;
  }
</style>

<svelte:head>
  <title>ZoeBot4</title>
</svelte:head>

<div class="img-container">
  <img src="zoe.png" alt="Zoe" />
</div>

<h1>{`Hey I'm Zoe Bot!`}</h1>

<p>{description}</p>

<h1>{`Why was I created?`}</h1>

<p>{creation}</p>

<div class="link-container" target="_blank" rel="noopener noreferrer">
  <a alt="r/zoemains" href="https://www.reddit.com/r/zoemains">
    psst, here's a secret portal to the community
  </a>
</div>

<h1>Need my help?</h1>
<p>{help}</p>

<div class="link-container">
  <a alt="about section" href="about">I want my awesome ZoeBot</a>
</div>
