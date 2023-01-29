<script>
	import { getContext } from 'svelte';
	import { TABS } from './Tabs.svelte';

	const tab = {};
	const { registerTab, selectTab, selectedTab } = getContext(TABS);

	registerTab(tab);
</script>

<style>
	button {
        border-bottom: 1px solid #fff;
        color: #7f7f7f;
        cursor: pointer;
        font-family: "Noto Serif KR",serif;
        font-size: 1rem;
        margin: 0 30px;
        padding: 20px 10px;
        background-color: #fff;
        border:none;
	}
	.selected {
		color:#964b00;
        border-bottom: solid 1px #964b00;
	}
</style>

<button class:selected="{$selectedTab === tab}" on:click="{() => selectTab(tab)}">
	<slot></slot>
</button>