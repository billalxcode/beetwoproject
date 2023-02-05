<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio:
						'Assalamualaikum. Perkenalkan, saya Billal Fauzan. Saya seorang programmer yang memiliki hobi dalam bidang ini. Keahlian saya meliputi beberapa bahasa pemrograman seperti Python, PHP, dan Javascript, serta bahasa scripting seperti HTML dan CSS. Kombinasi kemampuan ini membuat saya mampu berkontribusi dalam pengembangan aplikasi yang berkualitas.',
				},
				{
					id: 2,
					bio:
						'Saat ini, saya sedang menjalani karir sebagai Backend Developer. Saya sangat tertarik dengan bagian server-side dari sebuah aplikasi dan berusaha selalu mempelajari hal-hal baru untuk meningkatkan kualitas pekerjaan saya. Saya tinggal di Majalengka, tepatnya di kecamatan Maja, dan merasa sangat bahagia dapat memulai karir di kota kelahiran saya.',
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
				src="@/assets/images/profile.jpg"
				class="rounded-xl w-96"
				alt=""
			/>
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
