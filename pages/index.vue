<template>
  <div class="home-page">
    <section class="intro">
      <h1>Get the latest tech news!</h1>
    </section>
    <section class="featured-posts">
      <PostPreview
        id="1"
        thumbnail="https://media-exp1.licdn.com/dms/image/C4E1BAQEKkvWfkxxxww/company-background_10000/0/1597164510249?e=2159024400&v=beta&t=lMTf9_xn7UxGrawWjgOzfXc9-XhWkxqWD4at9c-tuFc"
        title="Hello there!"
        previewText="This is my first post"
      />
      <PostPreview
        id="2"
        thumbnail="https://media-exp1.licdn.com/dms/image/C4E1BAQEKkvWfkxxxww/company-background_10000/0/1597164510249?e=2159024400&v=beta&t=lMTf9_xn7UxGrawWjgOzfXc9-XhWkxqWD4at9c-tuFc"
        title="Hello there second!"
        previewText="This is my first post"
      />
      <PostPreview
        id="3"
        thumbnail="https://media-exp1.licdn.com/dms/image/C4E1BAQEKkvWfkxxxww/company-background_10000/0/1597164510249?e=2159024400&v=beta&t=lMTf9_xn7UxGrawWjgOzfXc9-XhWkxqWD4at9c-tuFc"
        title="Hello there third!"
        previewText="This is my first post"
      />
    </section>
  </div>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

export default {
  components: {
    PostPreview,
  },
}
</script>


<style scoped>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px black;
  box-sizing: border-box;
  border: 1px solid black;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
