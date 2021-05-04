<script>
	export let title, allContent;
</script>

<h1>{title}</h1>

<ul>
{#each allContent as page}
  {#if page.type == 'posts'}
    <li><a href="{page.path}">{page.filename}</a></li>
  {/if}
{/each}
</ul>

<style>
	h1 {
		font-family: Helvetica, sans-serif;
	}
</style>
