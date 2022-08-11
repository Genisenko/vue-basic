<template>
  <div>

    <div>
      <h1>{{ 2 + 2 + 2 }}</h1>
    </div>

    <div>
      <h1 v-if="propertyShow === true">Show if prop is set to true</h1>
      <h1 v-if="!propertyShow">Show if prop is set to false</h1>
    </div>

    <div>
      <div v-for="(post, index) in posts" :key="index">
        <ul>
          <li>
            <h1>Post Title: {{ post.title }}</h1>
            <h4>Post Description: {{ post.description }}</h4>
            <p>Post Content: {{ post.content }}</p>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      
      isLoading: true,
      propertyShow: false,
    
      posts: [
        {
          title: "The mystery of Toy Story",
          description: "Why Buzz Ligthyear pretended to be a toy when Andy cames?",
          content: "Why he did that if he believed that he was a real astronaut?",
        },
        {
          title: "What would you give for a kiss of 'la flaca'?",
          description: "I don't know you, but I would give anything for a kiss of 'la flaca'",
          content: "100lb of skin & bones",
        },
        {
          title: "Are we what we eat?",
          description: "If I drink a lot of alcohol, I'm alcoholic",
          content: "So, if I drink a lot of Fanta, am I Fantastic?",
        },
      ],
    };
  },
};
</script>


<style>
</style>
