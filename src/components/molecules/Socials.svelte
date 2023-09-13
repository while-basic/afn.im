<script>
	import Social from '../atoms/Social.svelte';
	import { user } from '../../util/discord';
</script>

<div class="socials-container">
	<Social icon="github" tip="xafn" link="https://github.com/while-basic" />
	<Social icon="discord" tip={user.username} link={`https://discord.com/users/${user.id}`} />
	<Social icon="email" tip="hey@afn.im" link="mailto:chris@chriscelaya.xyz" />
	<Social icon="kofi" tip="affan" link="https://chriscelaya.xyz" />
</div>

<style>
	.socials-container {
		display: flex;
		gap: 0.75rem;
	}
</style>
