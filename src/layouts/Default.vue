<template>
  <div class="layout">
    <header class="header">
      <strong>
        <g-link to="/">{{ $static.metadata.siteName }}</g-link>
        <!-- <g-link to="/hello-world">Hello world</g-link> -->
        <g-link to="/Laundrop" class="laundrop">Corona Crisis</g-link>
      </strong>
      <strong>
      <nav class="nav">
        <g-link class="nav__link" to="/">Home</g-link>
        <g-link class="nav__link" to="/about/">About</g-link>
      </nav>
      </strong>
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

<style>
.laundrop{
  padding: 0px 0px 0px 20px;
}
body {
  font-family: -apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
  margin:0;
  padding:0;
  line-height: 1.5;
  
}

.layout {
  /* max-width: 760px; */
  margin: 0 auto;
  /* padding-left: 20px;
  padding-right: 20px; */
  height: 900px;
  
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
  padding: 0px 0px 0px 20px;
  background: #4DC1C3;
}

.header :hover {
  color: blue;
  text-decoration: none;
}

.nav__link {
  margin-left: 20px;
  margin-right: 20px;
  
}
</style>
