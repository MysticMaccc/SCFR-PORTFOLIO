<script>
import DownloadCV from '../shared/DownloadCV.vue';
export default {
  components: { DownloadCV },
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio:
						'Greetings! I am Sherwin, a full stack web developer with an impressive track record spanning six years. My passion for crafting robust and efficient web solutions has driven me to master a diverse array of technologies.',
				},
				{
					id: 2,
					bio:
						'Throughout my career, I have consistently delivered high-quality, scalable, and user-centric web applications. My commitment to staying abreast of the latest industry trends ensures that the solutions I develop are not only cutting-edge but also aligned with the evolving needs of users. With a keen eye for detail and a dedication to excellence, I am well-equipped to tackle complex challenges and contribute to the success of any web development project.',
				},
			],
		};
	},
};
</script>

<template>
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About profile image -->
		<div class="w-full sm:w-1/4 mb-7 sm:mb-0">
			<img
				src="@/assets/images/profile.jpeg"
				class="rounded-xl w-96"
				alt=""
			/>
			<DownloadCV />
		</div>

		<!-- About details -->
		<div class="w-full sm:w-3/4 text-left">
			<p
				v-for="bio in bios"
				:key="bio.id"
				class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg"
			>
				{{ bio.bio }}
			</p>
		</div>

		

	</div>
</template>
