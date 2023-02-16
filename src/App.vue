<template>
  <div id="app" class="">
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
    <router-view />
  </div>
</template>
<script>
/* eslint-disable */
// eslint-disable-next-line
export default {
  name: "AppView",
  metaInfo() {
    return {
      title: "test meta data with vue",
      meta: [
        {
          vmid: "description",
          name: "description",
          content:
            "hello world, this is an example of adding a description with vueMeta"
        }
      ],
      // script: [
      //   { src: '<LINK_SOURCR>', async: true, defer: true, body: true }
      // ],
			// link: [
      //   {
      //     rel: 'REL',
      //     href: 'TAG_HREF'
      //   }
			// ]
    };
  },
  created(){
    const detected = navigator.userAgent
    console.log("userAgent", detected)
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
