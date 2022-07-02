<script>
    import {FeedbackStore} from '../stores';
    import {fade, scale} from 'svelte/transition';
    import FeedbackItem from './FeedbackItem.svelte';

</script>

{#each $FeedbackStore as fb (fb.id)}
<div transition:fade >
  <FeedbackItem item={fb} />
</div>

{/each}