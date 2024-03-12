<script>
    export let bg
    export let slideDir
    export let anchor
</script>

<section class="slide fade-6 kenBurns {slideDir}" id={anchor}>
    <div class="content">
        <div class="container">
            <div class="wrap">
                <slot />
            </div>
        </div>
    </div>
    <div
        class="background"
        style="background-image:url({bg})"
    ></div>
</section>