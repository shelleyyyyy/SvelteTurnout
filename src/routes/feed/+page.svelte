<script>
    // import Counter from "$lib/Counter.svelte";
    import Post from "$lib/feed/Post.svelte";

    let posts = [
        {
            "title": "Post 1",
            "description": "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Est adipisci fuga harum, ducimus similique distinctio saepe! In praesentium dolorum quis delectus totam explicabo aut quasi perferendis est. Inventore, distinctio laboriosam.",
            "author": "John Doe",
            "date": "2021-09-01",
            "info": [
                {
                    "title": "Likes",
                    "value": 10
                },
                {
                    "title": "Comments",
                    "value": 5
                },
                {
                    "title": "Views",
                    "value": 100
                },
            ]
        },
        {
            "title": "Post 2",
            "description": "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Est adipisci fuga harum, ducimus similique distinctio saepe! In praesentium dolorum quis delectus totam explicabo aut quasi perferendis est. Inventore, distinctio laboriosam.",
            "author": "John Doe",
            "date": "2021-09-01",
            "info": [
                {
                    "title": "Likes",
                    "value": 10
                },
                {
                    "title": "Comments",
                    "value": 5
                },
                {
                    "title": "Views",
                    "value": 100
                },
            ]
        }
    ]

</script>

<section>
    <h1 class="text-7xl font-bold pb-4" >Feed</h1>
    <div class="">
        {#each posts as post}
            <Post title={post.title} description={post.description} author={post.author} date={post.date} info={post.info}/>
        {/each}
    </div>
</section>

<style>

</style>