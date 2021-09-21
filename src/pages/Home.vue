<template>
	<div>
		<h3>This is a homepage.</h3>
		<p>
			Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptatum similique eligendi tempora expedita nam dolor nemo, ipsa dolorum blanditiis magnam cum nulla alias
			quisquam natus tempore temporibus. Doloribus, ipsum impedit ea magnam dignissimos sit. Eum voluptatum aperiam rem exercitationem dicta ea dolores tempore asperiores
			vero vitae dolorum quod quisquam, similique obcaecati eveniet, est non, animi possimus ab commodi consequuntur. Cumque harum deserunt neque sit, ratione provident
			dolore cupiditate. Molestias maiores commodi accusamus in quis voluptas aut, laudantium atque neque ex! Aut voluptate voluptas error ullam porro eos autem, deserunt
			ratione praesentium ab, nam necessitatibus tempore eius enim quos ipsa nemo!
		</p>
		<h3>ICONS</h3>
		<div class="icons">
			<IconAccessibility />
			<IconAccountBox />
			<Gear />
			<Bash />
		</div>
	</div>
</template>


<script>
import IconAccessibility from '~icons/carbon/accessibility';
import IconAccountBox from '~icons/mdi/account-box';
import Gear from '~icons/codicon/gear';
import Bash from '~icons/codicon/terminal-bash';
export default {
	components: {
		IconAccessibility,
		IconAccountBox,
		Gear,
		Bash,
	},
};
</script>

<style>
.icons {
	padding: 50px;
	font-size: 3rem;
	display: grid;
	gap: 20px;
	grid-template-columns: 1fr 1fr 1fr 1fr;
}
</style>
