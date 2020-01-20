<template>
  <Layout>

    <h1>{{ $page.work.title }}</h1>

    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Pariatur excepturi labore tempore expedita, et iste tenetur suscipit explicabo! Dolores, aperiam non officia eos quod asperiores
    </p>

  </Layout>
</template>

<page-query>
query work($id: ID!) {
  work: contentfulWorks(id: $id) {
    title
    url
  }
}
</page-query>

<script>
export default {
}
</script>

<style>
</style>
