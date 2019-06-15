<template>
<div>
  <intro />
  <specialties />
  <work />
  <working-process />
</div>
  
</template>

<script>
  import intro from '../components/intro';
  import specialties from '../components/specialties';
  import workingProcess from '../components/workingProcess';
  import work from '../components/work';

  export default {
    components: {
      intro, specialties, workingProcess, work
    }
  }
</script>
