<template>
  <Layout>
    <ul>
      <li v-for="work in $page.works.edges" :key="work.node.id">
        <g-link :to="`/works/${work.node.id}`">{{ work.node.title }}</g-link>
      </li>
    </ul>
  </Layout>
</template>

<page-query>
query getAllWorks {
  works: allContentfulWorks {
    edges {
      node {
        id
        title
        url
      }
    }
  }
}
</page-query>

<script>
</script>

<style>
</style>
