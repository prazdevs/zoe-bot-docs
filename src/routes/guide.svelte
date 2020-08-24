<script>
  const help = `There's this illusion of the reality, but it's not really really real, like it's beside and inside and inside and beside, but never on top... Nevermind, just kidding, but not really...`;

  const ahem = `Ahem. Let me help you use the right commands.`;
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

  code {
    font-size: 1.3rem;
  }

  p {
    font-size: 1.3rem;
  }

  div {
    font-size: 1.3rem;
    padding-left: 10px;
  }

  li {
    margin-top: 10px;
  }
</style>

<svelte:head>
  <title>ZoeBot4 | Guide</title>
</svelte:head>

<quote>{help}</quote>
<p style="text-align: right;">{ahem}</p>

<h1>{`You want to add a rule?`}</h1>
<ul>
  <li>
    <code>{`z!add zoemains #public`}</code>
    <div>
      I will automatically post zoemains submissions in the #public channel.
    </div>
  </li>
  <li>
    <code>{`z!add zoemains #public #mod`}</code>
    <div>
      I will automatically post zoemains submissions in the #mod channel and
      wait for a person with access to #mod to accept or reject the post (by
      reacting to it). If it is accepted i will post it in #public.
    </div>
  </li>
  <li>
    <code>{`z!add zoemains #public #mod 3600`}</code>
    <div>
      I will do exactly the same as above. But if you don't accept or reject the
      post within 3600 seconds (that's an hour, duh...), I will check on reddit:
      if the post is [deleted] or [removed], I won't post it, otherwise, I will!
    </div>
  </li>
</ul>

<h1>{`You want to remove a rule?`}</h1>
<ul>
  <li>
    <code>{`z!remove zoemains`}</code>
    <div>I will stop posting zoemains submissions. :(</div>
  </li>
</ul>

<h1>{`You want to list the existing rules?`}</h1>
<ul>
  <li>
    <code>{`z!get`}</code>
    <div>I will give you the rules you set for the server.</div>
  </li>
</ul>

<h1>{`You need help?`}</h1>
<ul>
  <li>
    <code>{`z!help`}</code>
    <div>I will give you a link to... uh... this page.</div>
  </li>
</ul>
