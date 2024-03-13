<script>
    export let slideDir
    export let animation
    export let text
    export let target
    export let id
</script>

<div class="main_div {slideDir} {animation} popupTrigger" data-popup-id={id}>
    <a href={target}><button type="submit" class="bold">{text}</button></a>
</div>

<style>
    @import '../../css/button.sanket.css';
</style>