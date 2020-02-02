
<template>
  <div class="settings" style="display:flex;height:100%">
    <SettingsMenu :options="options"/>
    <Timer />
      <Errorless />
      <UploadFile />
  </div>
</template>


<style scoped>
  .settings {
    display: flex;
  }
</style>


<script>
  import SettingsMenu from '../components/layout/SettingsMenu';
  import Timer from '../components/settings/Timer';
    import SettingsLinks from '@/views/SettingsLinks.js';
  
  export default {
    name: "Settings",
    components: {
      SettingsMenu,
      Timer,
      Errorless,
      UploadFile
    },
    data : function(){
        return {
            // Needs to be copy and pasted for each of the settings page
            'options' : SettingsLinks,
        }
    }
  }
</script>
