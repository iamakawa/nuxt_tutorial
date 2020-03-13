<template>
	<div class="container">
		<article>
			<h1 class="title">{{ post.title }}</h1>
			<p>{{ post.content }}</p>
		</article>
		<aside>
			<h3>links</h3>
			<ul>
				<li v-for="(related, id) in relatedPosts" :key="id">
					<!-- td><a :href="`/posts/${related.id}`">{{related.title}}</a></!-->
					<nuxt-link :to="{ name: 'posts-id', params: { id: related.id } }">{{related.title}}</nuxt-link>
				</li>
			</ul>
		</aside>
	</div>
</template>

<script>
export default {
	data() {
		return {
			id: this.$route.params.id,
			posts: [
				{
					id: "1",
					title: "one",
					content: "onet"
				},
				{
					id: "2",
					title: "two",
					content: "twoson"
				},
				{
					id: "3",
					title: "three",
					content: "treek"
				},
				{
					id: "4",
					title: "four",
					content: "fourside"
				}
			]
		};
	},
	computed: {
		post() {
			return this.posts.find(post => post.id === this.id);
		},
		relatedPosts() {
			return this.posts.filter(post => post.id !== this.id);
		}
	}
};
</script>

<style scoped></style>
