<template>
    <div>
        <h3>{{ 2 + 2 }}</h3>
        <br>
        <h3>{{ stringToPrint }}</h3>
        <br>
        <h3 v-show="thisIsTrue">
        This is being shown because the condition is true
        </h3>

        <h4 v-for="blogPost in blogPosts" :key="blogPost">The title of the book is {{ blogPost.title }}
        <br>
        The description of the book is {{ blogPost.description }}
        <br>
        The content of the book is {{ blogPost.content }}
        </h4>
    </div>
</template>

<script>
export default {
    data() {
        return {
            stringToPrint: "Aloha",

            thisIsTrue: true,

            blogPosts: [
                { title: "I Robot", description: "Book about robots", content: "Placeholder text 1"},
                { title: "How to kill a Mockingbird", description: "Book about rights", content: "Placeholder text 2"},
                {title: "The Man in the high Castle", description: "Book about authoritarian governments", content: "Placeholder text 3"}
            ],
        }
    }

}
</script>

<style>

</style>