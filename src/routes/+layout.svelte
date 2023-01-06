<script>
    import "../app.css";
    import { page } from "$app/stores";
    import "flowbite/dist/flowbite.css";
    console.log($page.route.id)
  </script>

  
  <nav class="
  flex flex-wrap justify-center
  w-80
  mt-16 mb-16 mx-auto
  py-0 px-5
  border-3px rounded-25em border-black
  bg-transparent 
  text-black text-lg font-bold">
      <a href="./" class= ' 
        {$page.route.id === '/' ? 'text-red-600' : ''} 
        m-3'>
        O mne
      </a>
      <a href="./projects" class= ' 
        {$page.route.id === '/projects' ? 'text-red-600' : ''} 
        m-3
        '>
        Projekty
      </a>    
      <a href="./contact" class= ' 
        {$page.route.id === '/contact' ? 'text-red-600' : ''} 
        m-3'>
        Kontakt
      </a>
    
</nav>



<slot />