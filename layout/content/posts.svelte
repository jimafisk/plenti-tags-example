<script>
  export let title, tags;
</script>

<h1>{title}</h1>


<div>
  <span>Tags:</span>
  {#each tags as tag}
    <span><a href="/tags/{tag}">{tag}</a></span>
  {/each}
</div>

<br>

<div><a href="/">Home</a></div>

<style>
  span {
    margin-right: 5px;
  }
</style>
