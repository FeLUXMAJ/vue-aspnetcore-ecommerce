<template>
<div class="app">
	<b-navbar toggleable="md" type="dark" variant="dark">
		<b-container>
			<b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
			<!-- The to navigates to the itnernal page (without the page load of an href) -->
			<b-navbar-brand to="/">PhoneShop</b-navbar-brand>
			<b-collapse is-nav id="nav_collapse">
				<b-navbar-nav>
					<b-nav-item to="/products">Products</b-nav-item>
				</b-navbar-nav>
			</b-collapse>
		</b-container>
	</b-navbar>
	
	<router-view />
</div>
</template>

<script>

export default {
	name: 'app'
}
</script>

<style lang="scss">
html,
body {
	height: 100vh;
}

div.app, div.page {
	height: 100% !important;
}

</style>
