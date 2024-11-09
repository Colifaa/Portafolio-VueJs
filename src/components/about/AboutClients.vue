<script>
import AboutClientSingle from './AboutClientSingle.vue';

export default {
	components: {
		AboutClientSingle,
	},
	data: () => {
		return {
			clientsHeading: 'Mis habilidades',
			clients: [
				{
					id: 1,
					title: 'Amazon',
					img: require('@/assets/images/brands/git.svg'),
				},
				{
					id: 2,
					title: 'Sony',
					img: require('@/assets/images/brands/html-css.svg'),
				},
				{
					id: 3,
					title: 'Adidas',
					img: require('@/assets/images/brands/java.svg'),
				},
				{
					id: 4,
					title: 'FILA',
					img: require('@/assets/images/brands/js.svg'),
				},
				{
					id: 5,
					title: 'NB',
					img: require('@/assets/images/brands/python.svg'),
				},
				{
					id: 6,
					title: 'SAMSUNG',
					img: require('@/assets/images/brands/mysql.svg'),
				},
				{
					id: 7,
					title: 'CANON',
					img: require('@/assets/images/brands/react.svg'),
				},
				{
					id: 7,
					title: 'PUMA',
					img: require('@/assets/images/brands/sql.svg'),
				},
			],
		};
	},
};
</script>

<template>
	<div class="mt-10 sm:mt-20">
		<p
			class="font-general-medium text-2xl sm:text-3xl text-primary-dark dark:text-primary-light"
		>
			{{ clientsHeading }}
		</p>
		<div class="grid grid-cols-2 sm:grid-cols-4 mt-10 sm:mt-14 gap-2">
			<AboutClientSingle
				v-for="client in clients"
				:key="client.id"
				:client="client"
				class="transform scale-75"
			/>
		</div>
	</div>
</template>
