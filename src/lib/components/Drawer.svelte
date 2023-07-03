<script lang="ts">
	import { base } from "$app/paths";
</script>

<div class="drawer drawer-end">
	<input id="my-drawer-4" type="checkbox" class="drawer-toggle" />
	<div class="drawer-content">
		<!-- Page content here -->
		<label for="my-drawer-4" class="drawer-button btn btn-primary">Open drawer</label>
	</div>
	<div class="drawer-side">
		<label for="my-drawer-4" class="drawer-overlay" />
		<ul class="menu p-4 w-80 bg-base-100 text-base-content">
			<!-- Sidebar content here -->
			<li><a href="{base}/">Sidebar Item 1</a></li>
			<li><a href="{base}/">Sidebar Item 2</a></li>
		</ul>
	</div>
</div>
