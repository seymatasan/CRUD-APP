<template>
  <q-item  clickable tag="a"  :to ="to">
    <q-item-section v-if="icon" avatar>
      <q-icon :name="icon" />
    </q-item-section>
    <q-item-section>
      <q-item-label>{{label}}</q-item-label>
    </q-item-section>
  </q-item>
</template>

<script>
export default {
  name: "EssentialLink",
  props: {
    label: {
      type: String,  
      required: true,
    },
    caption: {
      type: String,
      default: "",
    },
    icon: {
      type: String,
      default: "",
    },
    to: {
      type: String,
      default: "/",
    },
  },
};
</script>
