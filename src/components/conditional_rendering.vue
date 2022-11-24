<!--v-show is doing samething v-if. the differnt is use one over the other-->
<template id="ren">
  <div id="render" v-show="showElement">Using V-Show</div> <!--v-show always render in the DOM, only the display css property is show or hide the element-->
  <h2 v-if="showElement">Using V-if</h2><!--v-if mount the element onto the DOM, if condition is true, then if condition false remove the element in DOM-->
</template>

<script>
export default {
  name: 'conditional_rendering',
  props: {
    
  },
  data() {
    return {
        
        showElement: false //both the element show in the display & DOM// if give false, V-if not present in dom but v-show will present with css property set none.
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
 Input[type='text'],#btn1 {
    display: block;
    text-align: center;
    margin-top: 60px;
    width: 250px;
    padding: 6px 12px;
    font-size: 14px;
    line-height: 1.4 ;
    color: rgb(255, 255, 255);
    background-color:rgb(4, 42, 118) ;
    border: 1px solid #ccc;
    border-radius: 4px;
    margin : 0 auto;
 }
</style>
