<template>
<div style="padding:16px;">
  <button class="popup" v-on:click="to" >
    {{content}}
  </button>
  </div>
</template>


<style>  
  .popup {
    z-index: 9999;
    background: #fefefe;
    height: 200px;
    width: 300px;
    left: 0%;
    font-size: 28px;
    box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.5);
    border-width: 5px;
  }
</style>


<script>
export default {
  name : 'popup-btn-component',
  props : ['content', 'to']
}
</script>
