<template>
  <div>
    <p v-if="$fetchState.pending">Loading....</p>
    <p v-else-if="$fetchState.error">Error while fetching mountains</p>
    <ul v-else>
      <li v-for="(mountain, index) in mountains" :key="index">
        {{ mountain.title }}
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  data() {
    return {
      mountains: [],
    }
  },
  async fetch() {
    this.mountains = await fetch(
      'https://jsonplaceholder.typicode.com/todos'
    ).then((res) => res.json())
  },
}
</script>
