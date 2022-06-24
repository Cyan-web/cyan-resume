<div class="w-[120px] h-2 rounded-full overflow-hidden bg-gray-200">
    <div class="progress h-full {`w-[${$_progress}%]`}"></div>
</div>

<span>{$_progress}</span>

<script>
    import { tweened } from 'svelte/motion'
    import { cubicOut } from 'svelte/easing'

    export let progress = 0

    $: _progress = tweened(progress, {
        duration: 400,
        easing: cubicOut
    })
</script>

<style>
    .progress {
        /*background-image: linear-gradient(45deg, #ffd591, #ffd591);*/
        background-image: -webkit-repeating-linear-gradient(-45deg, #f20, #ffd591);
        background-size: 100% 100%;
    }
</style>
