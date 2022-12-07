<template>
    <div class="banner-card" v-bind:class="bannerStyle">
        <img v-bind:src="img" v-bind:alt="img + ' image'">
        <div class="banner-card__status" :style="'background-color: ' + statusBgColor">
            <span :style="'color: ' + statusColor">{{ title }}</span>
        </div>
    </div>
</template>

<script>
export default {
    name: "BannerCard",
    props: [
        'img',
        'statusTitle',
        'bannerStyle',
        'title',
        'statusColor',
        'statusBgColor'
    ]
}
</script>

<style scoped>
img {
    width: 100%;
    object-fit: cover;
}
.banner-card {
    position: relative;
    border-radius: 16px;
    overflow: hidden;
    display: flex;
    flex-shrink: 0;
}
.banner-card__status {
    border-radius: 24px;
    padding: 8px 12px;
    position: absolute;
    top: 12px;
    right: 12px;
}
</style>