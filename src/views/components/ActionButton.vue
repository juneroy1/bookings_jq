<template>
  <div>
    <button @click="saveItem">Save</button>
    <button>Delete</button>
  </div>
</template>

<script>

export default {
  name: "ActionButton",
  setup(props, { emit }) {
    const saveItem = ( () => {
        emit('saveItem')
    })
    return {saveItem};
  },
};
</script>

<style lang="scss" scoped></style>
