<script setup lang="ts">
	import { ref } from 'vue'

	const props = defineProps({
		name: {
			type: String,
			default: 'Component' /*PinegrowComponentTemplate*/,
		},
	})

	const suffix = ref('placeholder')
</script>
<template>
    <div class="p-4">
        <div class="max-w-sm rounded overflow-hidden shadow-lg mb-4">
            <img class="w-full" src="https://tailwindcss.com/img/card-top.jpg" alt="Sunset in the mountains"/>
            <div class="px-6 py-4 pb-2">
                <div class="font-bold text-xl mb-2">The Coldest Sunset</div>
                <p class="text-gray-700 text-base">
					Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maiores et
					perferendis eaque, exercitationem praesentium nihil. </p>
            </div>
            <div class="px-6 py-4"><span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 hover:bg-gray-300 mr-2">#photography</span><span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 hover:bg-gray-300 mr-2">#travel</span><span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 hover:bg-gray-300">#winter</span>
            </div>
        </div><a href="/about"> <button class="bg-primary-900 font-bold hover:bg-blue-700 px-4 py-2 rounded text-fuchsia-500">
                <slot>Button</slot>
            </button> </a>
    </div>
</template>
<style scoped></style>
