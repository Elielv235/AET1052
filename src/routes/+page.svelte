<script lang="ts">
	// Global styles
	import '../Styling/global.scss';

	// Section imports
	import Section from '../Components/Section.svelte';
	import PeopleGrid from '../Components/peopleGrid.svelte';
	import Welcome from '../Components/Sections/Welcome.svelte';
	import NavBar from '../Components/NavBar.svelte';
	import About from '../Components/Sections/About.svelte';
</script>

<NavBar />

<Section id="welcome">
	<Welcome />
</Section>

<Section id="about">
	<About />
</Section>
<Section id="people">
	<PeopleGrid />
</Section>
