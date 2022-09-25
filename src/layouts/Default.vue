<template>
  <div class="layout">
    <header class="header">
      <nav class="nav">
<!--        <g-link class="nav__link" to="/">Home</g-link>-->
      </nav>
    </header>
    <slot/>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>
<script>
export default {
  metaInfo: {
    link: [
      {
        rel: 'stylesheet',
        href: 'https://cdn.jsdelivr.net/npm/bootstrap-icons@1.9.1/font/bootstrap-icons.css'
      }
    ]
  }
}
</script>