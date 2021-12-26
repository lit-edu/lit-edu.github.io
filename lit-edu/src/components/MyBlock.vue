<template>
  <a class="block">
    <div class="block-avatar">
      <!-- <img src=".././assets/avatars/1.png" alt="icon"> -->
      <b-img v-bind="mainProps" rounded="circle" alt="Circle image"></b-img>
    </div>
    <div class="block-title">
      洛阳理工电器学院
    </div>      
  </a>
</template>

<script>
  export default {
    name: "MyBlock",
    data() {
      return {
        mainProps: {blank: true, blankColor: '#dfdfdf',width: 48, height: 48, class: 'block-img' }
      }
    }
  }
</script>

<style scoped>
.block {
  margin: 6px;
  padding: 8px 12px;
  width: 100px;
  height: 100px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-color: #fff;
  box-shadow: 0px 4px 4px rgba(186, 185, 247, 0.17);
  border-radius: 11px;
  font-size: 12px;
  font-family: Source Sans Pro;
  font-style: normal;
  font-weight: 900;
  color: #3F51B5;
  text-decoration:none;
}
.block-img {
  margin-bottom: 9px;
}
.block-title{
  text-align: center;
}
</style>