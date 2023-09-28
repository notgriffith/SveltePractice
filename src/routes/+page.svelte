<!-- <h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p> -->
<script>
  import AddButton from './AddButton.svelte';

  import PostListing from './PostListing.svelte';
  import Header from './Header.svelte';
  import Footer from './Footer.svelte';
</script>
<!-- <div class="block lg:hidden">
    <button
    on:click={change}
      class="flex items-center px-3 py-2 rounded text-black-500 hover:text-black-400"
    >
      <svg
        class={`fill-current h-3 w-3 ${state ? "hidden" : "block"}`}
        viewBox="0 0 20 20"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" />
      </svg>
      <svg
        class={`fill-current h-3 w-3 ${state ? "block" : "hidden"}`}
        viewBox="0 0 20 20"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path d="M10 8.586L2.929 1.515 1.515 2.929 8.586 10l-7.071 7.071 1.414 1.414L10 11.414l7.071 7.071 1.414-1.414L11.414 10l7.071-7.071-1.414-1.414L10 8.586z" />
      </svg>
    </button>
</div> -->
<Header/>


<PostListing/>
<AddButton/>
<Footer/>

<style>
    @import './global.css';

</style>