<template>
<div>
  
  <p class="demo">
    prop = {{ msg }}
  </p>
  <p>
    msg 2 = {{msg2}}
  </p>
</div>
</template>

<script>
  export default {
    props: ['msg'],
    data() {
      return {
        msg2: 'Hello this is <demo-component>'
      }
    }
  }
</script>

