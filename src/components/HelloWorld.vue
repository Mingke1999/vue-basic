<template>
  <div class="hello">
    <p>{{message}}</p> <!--binding text-->
    <div v-html="mingkeLink"></div> <!--binding html-->
    <p v-bind:class="onActive">Highlight</p> <!--binding class attribute-->
    <p v-bind:id="vid">BindingID</p> <!--binding class id-->
    <input :disabled="isAbled" value="Bool Attribute Disabled"/> <!--binding boolean attribute-->
    <div v-bind="objectOfAttrs">Multiple Binding Dynamic</div> <!--binding multiple attributes-->
    <p>{{number>10?"Number is bigger than 10":"Number isn't bigger than 10"}}</p> <!--Expression only not statement-->
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data(){ //declare a data source
    return{
      message:'Text:hello Vue from Mingke',
      mingkeLink:'<a href="https://github.com/Mingke1999">MingkeGit</a>',
      onActive:'active',
      vid:'007',
      isAbled:'false',
      objectOfAttrs: {id: 'container',class: 'wrapper'},
      number:10,
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
