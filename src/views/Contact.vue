<script>
import feather from 'feather-icons';
// import ContactForm from '@/components/contact/ContactForm.vue';
import ContactDetails from '@/components/contact/ContactDetails.vue';

export default {
	components: {
		// ContactForm,
		ContactDetails,
	},
	data: () => {
		return {
			contacts: [
				{
					id: 1,
					name: 'B7 L45 Birmingham Village, Pulo, Cabuyao, Laguna',
					icon: 'map-pin',
				},
				{
					id: 2,
					name: 'cosmicsher96@gmail.com',
					icon: 'mail',
				},
				{
					id: 3,
					name: 'sherwinroxas602@gmail.com',
					icon: 'mail',
				},
				{
					id: 4,
					name: '(+63)994-215-2415',
					icon: 'phone',
				},
				{
					id: 5,
					name: '(+63)950-909-8702',
					icon: 'phone',
				},
			],
		};
	},
	mounted() {
		feather.replace();
	},
	updated() {
		feather.replace();
	},
	methods: {},
};
</script>

<template>
	<div
		class="container mx-auto flex flex-col-reverse md:flex-row py-5 md:py-10 md:mt-10 justify-center"
	>
		<!-- Contact form -->
		<!-- <ContactForm /> -->

		<!-- Contact details -->
		<ContactDetails :contacts="contacts" />
	</div>
</template>
