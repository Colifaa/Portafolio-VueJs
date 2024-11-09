<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio:
						"Hola, Soy Mathez Jorge Alí "
				},
				{
					id: 2,
					bio:
						'Como desarrollador web, estoy comprometido a crear sitios web de alta calidad. aplicaciones que satisfagan las necesidades de mis clientes. Con años de experiencia en desarrollo web full-stack, me especializo en el uso de React.js, Next js, JavaScript, Solidity, MongoDB, Express.js y Node.js para crear aplicaciones web escalables y robustas.',
				},
				{
					id: 3,
					bio:
						'con experiencia en distintas tecnologías de desarrollo web como HTML, CSS, Javascript, React, Redux, Node.js, SQL React.js, Next js, MongoDB, Express.js.💻 Además de mi experiencia en desarrollo web, también tengo habilidades adicionales que me hacen un candidato aún más valioso para cualquier proyecto, como la música y el trading de criptomonedas. 📈📊🎸🎧',
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
      <img src="../../assets/images/Jorge.png" class="rounded-xl w-96" alt="" />
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
