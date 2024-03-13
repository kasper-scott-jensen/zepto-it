<script>
  export let source
  export let id
</script>

<div class="popup autoplay" data-popup-id={id}>
  <div class="content">
    <div class="container">
      <div class="wrap">
        <div class="fix-10-12">
          <div class="embedVideo popupContent">
            <!-- svelte-ignore a11y-media-has-caption -->
            <video
              src={source}
              autoplay
            ></video>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
