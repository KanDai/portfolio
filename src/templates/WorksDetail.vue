<template>
  <Layout>
    <h1>{{ $page.work.title }}</h1>
    <p>
      {{ $page.work.description }}
    </p>
  </Layout>
</template>

<page-query>
query work($id: ID!) {
  work: contentfulWorks(id: $id) {
    title
    url
    description
  }
}
</page-query>

<script>
</script>

<style>
</style>
