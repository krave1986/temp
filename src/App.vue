<template>
	<div id="app">
		<label for="catalogs">规则集：</label>
		<select id="catalogs" v-model="bbc">
			<optgroup label="A">
				<option value="1">ppp</option>
				<option value="2">qqq</option>
			</optgroup>
			<optgroup label="B">
				<option value="3">ppp</option>
				<option value="4">qqq</option>
			</optgroup>
			<optgroup label="C">
				<option value="5">ppp</option>
				<option value="6">qqq</option>
			</optgroup>
		</select>
	</div>
</template>

<script>
export default {
	name: "app",
	data() {
		return {
			bbc: "fff"
		};
	},
	watch: {
		bbc: function(nv) {
			console.log(nv);
		}
	},
	mounted() {
		console.log(this.bbc);
	}
};
</script>

<style>
body {
	margin: 0;
}
select {
	appearance: none;
	width: 200px;
	height: 32px;
	border-radius: 4px;
	text-indent: 4px;
	border: 1px solid rgba(217, 217, 217, 1);
}
</style>
