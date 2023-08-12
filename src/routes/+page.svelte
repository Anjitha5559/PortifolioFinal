<script>
	import Header from './pages/header.svelte';
	import MainBody from './pages/mainBdy.svelte';
	import AboutMe from './pages/AboutMe.svelte';
	import Know from './pages/knowl.svelte';
	import Project from './pages/Projects.svelte';
	import ContactMe from './pages/ContactMe.svelte';
	import Timeline from './pages/timeline.svelte';
</script>

<div id="APP_Body">
	<Header />
	<MainBody />
	<AboutMe />
	<Know />
	<Project />
	<Timeline />
	<ContactMe />
</div>

<style>
	#APP_Body {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		width: 100%;
		height: 100%;
		background-color: #110028;
	}
</style>
