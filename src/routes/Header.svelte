<script>
      import XImage from './X.png';
      import {onMount} from 'svelte';
      let isHeaderOpen = true; // Initially, the header is open

// Function to toggle the header state
function toggleHeader() {
  isHeaderOpen = !isHeaderOpen;
}
   onMount(()=>{
    console.log('mounted')
// Event listener to handle scrolling
window.addEventListener("scroll", () => {
  const scrollY = window.scrollY;

  // Check if the user has scrolled down enough to close the header
  if (scrollY > 100) {
    console.log('done')
    toggleHeader();
  }
});
   })

</script>

<div class:closed={isHeaderOpen} class='header p-5 bg-[#000000]' >
    <div class="flex flex-row place-content-between items-center">
        <div class="">
          <div class="rounded-full h-8 w-8 flex items-center justify-center bg-purple-500 text-white text-center">g</div>
        </div>
        <div class="">
            <a href="" class="  text-gray-900">
                <img class="w-8" src={XImage} alt="X Image" />
              </a>
        </div>
        <div class="w-8">
          <!-- <a href="" class="  text-gray-900">
              <img class="w-8" src={XImage} alt="X Image" />
            </a> -->
      </div>
    </div>
</div>




<style>
  .header {
    height: 100px; /* Adjust the height according to your design */
    transition: transform 0.3s ease; /* Smooth transition effect */
    transform: translateY(0); /* Initially, the header is not translated */
  }

  /* Apply a translation when the header is closed */
  .header.closed {
    transform: translateY(-100%); /* Move the header up by its own height */
  }
</style>

