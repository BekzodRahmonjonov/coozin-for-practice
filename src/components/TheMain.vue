<template>
    <main class="container">
        <div class="banner">
            <banner-card
                :img="'https://picsum.photos/200/300'"
                title="Посуда"
                banner-style="banner-1"
                status-bg-color="#F0F9FF"
                status-color="#0284C7"
            />
            <div class="banner__item banner__item_col">
                <div class="banner__item">
                    <div
                        v-for="(data, index) in bannerData.slice(0, 2)"
                        :key="index"
                    >
                        <banner-card
                            :img="data.img"
                            :title="data.title"
                            :banner-style="data.bannerStyle"
                            :status-bg-color="data.statusBgColor"
                            :status-color="data.statusColor"
                        />
                    </div>
                </div>

                <div class="banner__item">
                    <div
                        v-for="(data, index) in bannerData.slice(-2)"
                        :key="index"
                    >
                        <banner-card
                            :img="data.img"
                            :title="data.title"
                            :banner-style="data.bannerStyle"
                            :status-bg-color="data.statusBgColor"
                            :status-color="data.statusColor"
                        />
                    </div>
                </div>
            </div>
        </div>

    </main>
</template>

<script>
import BannerCard from "@/components/BannerCard";

export default {
    name: "TheMain",
    components: {BannerCard},
    data() {
        return {
            bannerData: [
                {
                    img: 'https://picsum.photos/700/1000',
                    title: 'Кондитерская',
                    bannerStyle: 'banner-2',
                    statusBgColor: '#FEF2F2',
                    statusColor: '#DC2626'
                },
                {
                    img: 'https://picsum.photos/800/1100',
                    title: 'Домашняя еда',
                    bannerStyle: 'banner-3',
                    statusBgColor: '#FFF8F5',
                    statusColor: '#FF6600'
                },
                {
                    img: 'https://picsum.photos/900/1200',
                    title: 'Ручные изделия',
                    bannerStyle: 'banner-4',
                    statusBgColor: '#F5F3FF',
                    statusColor: '#7C3AED'
                },
                {
                    img: 'https://picsum.photos/1000/1300',
                    title: 'Цветы',
                    bannerStyle: 'banner-5',
                    statusBgColor: '#ECFDF5',
                    statusColor: '#059669'
                }
            ]
        }
    }
}
</script>

<style scoped>
.banner, .banner__item {
    display: flex;
    gap: 16px;
}

.banner__item_col {
    flex-direction: column;
}

.banner-1 {
    width: 312px;
    height: 325px;
}

.banner-2 {
    width: 384px;
    height: 154px;
}

.banner-3 {
    width: 488px;
    height: 154px;
}

.banner-4 {
    width: 472px;
    height: 154px;
}

.banner-5 {
    width: 400px;
    height: 154px;
}
</style>