<style>
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
</style>

<script>
	export let type = "default"
	export let name = "Button"
</script>

{#if type=="default"}
<button class="bg-blue-600 text-white px-40 py-3 m-3 rounded-full font-semibold hover:bg-blue-700">{name}</button>
{/if}

{#if type=="active"}
<button class="bg-blue-700 text-white px-40 py-3 m-3 rounded-full font-semibold">{name}</button>
{/if}

{#if type=="disabled"}
<button class="bg-gray-300 text-gray-500 px-40 py-3 m-3 rounded-full font-semibold">{name}</button>
{/if}