<script lang="ts">
	// Global styles
	import '../Styling/global.scss';

	// Section imports
	import Section from '../Components/Section.svelte';
	import ImageGrid from '../Components/imageGrid.svelte';
	import Welcome from '../Components/Sections/Welcome.svelte';
	import NavBar from '../Components/NavBar.svelte';
	import About from '../Components/Sections/About.svelte';
	import PeopleGrid from '../Components/Sections/peopleGrid.svelte';
	import Research from '../Components/Sections/Research.svelte';
</script>

<NavBar />

<Section id="home">
	<Welcome />
</Section>

<Section id="about">
	<About />
</Section>
<Section id="Research">
	<Research />
</Section>
<Section id="Team">
	<PeopleGrid />
</Section>
<Section id="Media">
	<ImageGrid />
</Section>
