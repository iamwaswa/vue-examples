<template>
  <div>
    <slot :user="user">
      {{ user.lastName }}
    </slot>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: `default-slot`,
  data: function() {
    return {
      user: {
        firstName: `Steve`,
        lastName: `Jobs`
      }
    };
  }
});
</script>
