<template>
  <b-container fluid class="profileImg">
    <b-row>
      <b-col>
        <b-img rounded="circle" width="175" height="175" blank-color="#777" class="m-1" center thumbnail fluid src="https://picsum.photos/250/250/?image=54" alt="Thumbnail" ></b-img>
      </b-col>
    </b-row>
  </b-container>

</template>

<script>
    export default {
  name: 'profilImage'
    }
</script>

<style scoped>
.profileImg {
  margin-top: 5%;
}
</style>
