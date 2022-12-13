<template>
	<div>
		<!--<h1>{{ $t('hello', { name: 'vue-i18n' }) }}</h1>
		<select v-model="$colorMode.preference">
			<option value="system">System</option>
			<option value="light">Light</option>
			<option value="dark">Dark</option>
			<option value="sepia">Sepia</option>
		</select>-->
		<NuxtLayout>
			<NuxtPage />
		</NuxtLayout>
	</div>
</template>

<script setup>
import { Calendar } from 'v-calendar';
//const colorMode = useColorMode()
//console.log(colorMode.preference)
useHead({
	title: "Santhi Bakery",
	meta: [
		{
			name: "description",
			content: "SANTHI BAKERY was established by Mr.S. GOPAL(Founder). Since its inception it is growing from strength to strength in the bakery business.",
		},
		{
			property: "og:title",
			content: "Santhi Bakery",
		},
		{
			property: "og:description",
			content: "SANTHI BAKERY was established by Mr.S. GOPAL(Founder). Since its inception it is growing from strength to strength in the bakery business.",
		},
		{
			property: "og:image",
			content: "/",
		},
		{
			property: "og:type",
			content: "https://www.santhibakery.in",
		},
		{
			property: "og:site_name",
			content: "Santhi Bakery",
		},
	],
});
</script>
