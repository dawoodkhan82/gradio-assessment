<script context="module" lang="ts">
	import type { FileData } from "@gradio/upload";
	export interface AudioData extends FileData {
		crop_min?: number;
		crop_max?: number;
	}
</script>

<script lang="ts">
	import { createEventDispatcher } from "svelte";
	import { BlockLabel } from "@gradio/atoms";

	import { Music } from "@gradio/icons";

	export let value: null | { name: string; data: string } = null;
	export let label: string;
	export let name: string;
	export let show_label: boolean;

	const dispatch = createEventDispatcher<{
		change: AudioData;
		play: undefined;
		pause: undefined;
		ended: undefined;
	}>();

	$: value &&
		dispatch("change", {
			name: name,
			data: value?.data
		});
</script>

<BlockLabel {show_label} Icon={Music} label={label || "Audio"} />
{#if value === null}
	<div class="h-full min-h-[8rem] flex justify-center items-center">
		<!-- <img src={audio_icon} alt="" class="h-6 opacity-20" /> -->
		<div class="h-5 dark:text-white opacity-50"><Music /></div>
	</div>
{:else}
	<audio
		class="w-full h-14 p-2 mt-7"
		controls
		preload="metadata"
		src={value.data}
		on:play
		on:pause
		on:ended
	/>
{/if}
