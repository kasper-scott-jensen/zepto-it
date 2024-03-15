<script>
  export let source
  export let id
  export let title
</script>

<div class="popup autoplay" data-popup-id={id}>
  <div class="content">
    <div class="container">
      <div class="wrap">
        <div class="fix-10-12">
          <div class="embedVideo popupContent">
            <iframe src={source} title={title} frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
