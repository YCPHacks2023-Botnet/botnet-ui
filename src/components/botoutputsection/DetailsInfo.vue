<script setup>
import DetailsFrame from './DetailsFrame.vue'
</script>

<template>
    <DetailsFrame>
        <template #botname>Name</template>
        <template #botID>ID</template>
        <template #CPU>cpu info</template>
        <template #RAM>ram info</template>
        <template #status>Activity Status</template>
        <template #currenttask>Current Task</template>
        <template #taskparams>param1, param2</template>
    </DetailsFrame>
</template>