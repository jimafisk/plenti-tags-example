<script>
  export let name, allContent;  
</script>

<h1>Term: {name}</h1>

<h3>All posts tagged with "{name}":</h3>
<ul>
{#each allContent as content}
  {#if content.type == 'posts'}
    {#each content.fields.tags as tag}
      {#if tag == name}
        <li><a href="{content.path}">{content.filename}</a></li>
      {/if}
    {/each}
  {/if}
{/each}
</ul>

<br>

<div><a href="/">Home</a></div>
