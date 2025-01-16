<template>
  <v-app-bar elevation="0" class="">
    <v-container fluid>
      <ul class="d-flex align-center mr-10">
        <li><router-link to="">get started now</router-link></li>
        <li><router-link to="" class="log-in-btn">login</router-link></li>
      </ul>
    </v-container>
  </v-app-bar>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
/*start navbar style*/
ul {
  display: flex;
  justify-content: end;
  gap: 20px;
  li {
    list-style: none;
  }
  a {
    color: #000;
    text-transform: capitalize;
    font-weight: 500;
  }
  .log-in-btn {
    text-decoration: none !important;
    background: #f2f2f2;
    border-radius: 13px;
    padding: 3px 15px;
  }
}
/*Resposive Mopile Screen*/
@media (max-width: 591px) {
  nav {
    li {
      a {
        font-size: 14px;
      }
    }
  }
}
/*Resposive Mopile Screen*/
/*end navbar style*/
</style>
