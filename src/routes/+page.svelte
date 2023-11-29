<script>
  export let data;
</script>
<ul>
  {#each data.blog as post}
  <div class="blog-post">
  <h2>{post.blog_title}</h2>
  <div class="flexbox">
    <p class="author"><strong>{post.blog_author}</strong></p>
    <p class="tags">{post.blog_tag}</p>
  </div>
  <p>{post.blog_content}</p>
  <p class="date">{post.blog_date}</p>
  </div>
  {/each}
</ul>

<style>
  .blog-post {
    max-width: 60ch;
    background-color: burlywood;
    padding: 1rem;
    border-radius: 1rem;
    
  }
  .flexbox {
    display: flex;
    justify-content: space-between;
  }
  .tags {
    background-color: rgb(149, 224, 233);
    padding: .25rem;
    border-radius: .25rem;
    color: rgb(243, 243, 243);
  }
  .author {
    padding: .25rem;
  }
  .date {
    text-decoration: underline;
    text-align: right;
  }
</style>