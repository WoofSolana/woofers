<template>

    <div>
        <nuxt />
    </div>
</template>

<script>
export default {
  layout: "empty",
  data () {
    return {
    showMobileMenu: false
    }
}
};
</script>

<style scoped>
    .navbar {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
</style>