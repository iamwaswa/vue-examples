<template>
  <div>
    <DefaultSlot>
      <template v-slot:default="{ user }">
        {{ user.firstName }}
      </template>
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
