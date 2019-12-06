<template>
  <div>
    <DefaultSlot v-slot="{ user }">
      {{ user.firstName }}
    </DefaultSlot>
  </div>
</template>

<script>
import DefaultSlot from "@/components/default-slot";

export default {
  name: `home`,
  components: {
    DefaultSlot
  }
};
</script>
