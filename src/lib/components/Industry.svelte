<script>
    export let img, title, content;
  </script>
  
  <div class="flex flex-col w-72 bg-gray-50   pt-8">
    <img src={img} alt="" class="w-60 mx-auto" />
    <span class="text-center"><b>{title}</b></span>
    <p class="text-center px-8">
      {content}
    </p>
  </div>
  