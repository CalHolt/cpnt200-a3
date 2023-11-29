<script>
  export let data;
</script>
<ul>
  {#each data.blog as post}
  <h3>{post.blog_title}</h3>
  {/each}
</ul>