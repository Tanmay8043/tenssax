<script>
    export let img, title, content;
  </script>
  
  <div class="flex flex-col">
    <img src={img} alt="" />
    <span class="text-center"><b>{title}</b></span>
    <p class="text-center">
      {content}
    </p>
  </div>
  