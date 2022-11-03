<template>
    <div>
        <Suspense>
            <AsyncCityViewVue />
            <template #fallback>
                <CityViewSqueleton />
            </template>
        </Suspense>
    </div>
</template>

<script setup>
import AsyncCityViewVue from '../components/AsyncCityView.vue';
import CityViewSqueleton from '../components/CityViewSqueleton.vue';
</script>
