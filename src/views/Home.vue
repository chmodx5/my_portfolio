<template>
<div>
  <intro />
  <specialties />
  <working-process />
</div>
  
</template>

<script>
  import intro from '../components/intro';
  import specialties from '../components/specialties';
  import workingProcess from '../components/workingProcess';

  export default {
    components: {
      intro, specialties, workingProcess
    }
  }
</script>
