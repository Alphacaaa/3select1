<script>
import { RouterLink } from 'vue-router'
export default {
    components: {
        RouterLink
    }
}
</script>

<template>
<div class="headerArea">
    <RouterLink class="routeItem" to="/">首頁</RouterLink>
    <RouterLink class="routeItem" to="/firstPage">第一</RouterLink>
</div>
</template>

<style scoped lang="scss">
.headerArea{
    height: 100%;
    width: 100%;
    border: 1px solid black;
}
</style>