<template>
	<footer class="footer">
		<div class="container py-2">
			<div class="d-flex justify-content-between">
				<Version v-bind="version" />
				<Savings v-bind="savings" />
			</div>
		</div>
	</footer>
</template>

<script>
import "@h2d2/shopicons/es/filled/testtube";

import Version from "./Version.vue";
import Savings from "../Savings/Savings.vue";

export default {
	name: "Footer",
	components: { Version, Savings },
	props: {
		version: Object,
		savings: Object,
	},
};
</script>
