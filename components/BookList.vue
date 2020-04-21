<template>

  <div>
    <b-card-group columns>

      <b-card
        :title="book.title"
        img-src="https://placekitten.com/g/400/450"
        img-alt="Image"
        img-top
        v-for="book in books"
      >
        <b-card-text>
          {{book.author}}
        </b-card-text>
      </b-card>

    </b-card-group>
  </div>

</template>

<script lang="ts">
  import Vue from 'vue'

  export default Vue.extend({
    name: 'BookList',
    data() {
      return {
        books: [
          {
            id: 1,
            title: 'Winnie The Pooh',
            author: 'A. A. Milne',
            publishedAt: 2018
          },
          {
            id: 2,
            title: 'Norwegian Wood',
            author: 'H. Murakami',
            publishedAt: 2020
          },
          {
            id: 3,
            title: 'Dziady',
            author: 'A. Mickiewicz',
            publishedAt: 2020
          }
        ]
      }
    }
  })
</script>
