<script>
  import Header from './Header.svelte';

 
        let state = false;
        let items = [
          {id:0, name:'saad',post:"hello this my first tweet"},
          {id:2, name:'waqas',post:"Just over 12 hours to go until the rankings update! Who will be No. 1 in the ODI batting rankings in the morning? Shubman Gill or Babar Azam? "},
          {id:3, name:'kamran',post:"hello this my third tweet"},
          {id:4, name:'ali',post:"hello this my last tweet"},
          {id:2, name:'waqas',post:"Just over 12 hours to go until the rankings update! Who will be No. 1 in the ODI batting rankings in the morning? Shubman Gill or Babar Azam? "},
          {id:3, name:'kamran',post:"hello this my third tweet"},
          {id:4, name:'ali',post:"hello this my last tweet"},
          {id:2, name:'waqas',post:"Just over 12 hours to go until the rankings update! Who will be No. 1 in the ODI batting rankings in the morning? Shubman Gill or Babar Azam? "},
          {id:3, name:'kamran',post:"hello this my third tweet"},
          {id:4, name:'ali',post:"hello this my last tweet"},
          {id:2, name:'waqas',post:"Just over 12 hours to go until the rankings update! Who will be No. 1 in the ODI batting rankings in the morning? Shubman Gill or Babar Azam? "},
          {id:3, name:'kamran',post:"hello this my third tweet"},
          {id:4, name:'ali',post:"hello this my last tweet"},
          {id:2, name:'waqas',post:"Just over 12 hours to go until the rankings update! Who will be No. 1 in the ODI batting rankings in the morning? Shubman Gill or Babar Azam? "},
          {id:3, name:'kamran',post:"hello this my third tweet"},
          {id:4, name:'ali',post:"hello this my last tweet"},
          {id:2, name:'waqas',post:"Just over 12 hours to go until the rankings update! Who will be No. 1 in the ODI batting rankings in the morning? Shubman Gill or Babar Azam? "},
          {id:3, name:'kamran',post:"hello this my third tweet"},
          {id:4, name:'ali',post:"hello this my last tweet"},
          {id:2, name:'waqas',post:"Just over 12 hours to go until the rankings update! Who will be No. 1 in the ODI batting rankings in the morning? Shubman Gill or Babar Azam? "},
          {id:3, name:'kamran',post:"hello this my third tweet"},
          {id:4, name:'ali',post:"hello this my last tweet"},
          {id:2, name:'waqas',post:"Just over 12 hours to go until the rankings update! Who will be No. 1 in the ODI batting rankings in the morning? Shubman Gill or Babar Azam? "},
          {id:3, name:'kamran',post:"hello this my third tweet"},
          {id:4, name:'ali',post:"hello this my last tweet"},
          {id:2, name:'waqas',post:"Just over 12 hours to go until the rankings update! Who will be No. 1 in the ODI batting rankings in the morning? Shubman Gill or Babar Azam? "},
          {id:3, name:'kamran',post:"hello this my third tweet"},
          {id:4, name:'ali',post:"hello this my last tweet"},
        ]
    function change(){
        state=!state;
        console.log('this is state',state)
    }
</script>

<div class='border-b-[.01rem] border-gray-700  bg-[#000000]' >
  <div class="flex flex-row place-content-between  custom-border items-center">
      <div class="w-1/2 text-center pb-5 underline">
        <h2 class="text-white underline" style="text-underline-offset: 20px; text-decoration-thickness: 4px; text-decoration-color:#4D9BF0">For you</h2>
      </div>
     
      <div class="w-1/2 text-center pb-5">
        <h2 class="text-white">Following</h2>
    </div>
  </div>
  <ul>
    {#each items as item (item.id)}
    <li class=" px-5 py-2 flex custom-border">
      <div class="">
        <div class="rounded-full h-8 w-8 flex items-center justify-center bg-purple-500 text-white text-center ">   {item.name.charAt(0).toUpperCase()}</div>
      </div>
      <div class="ml-3">
        <span class="text-white block font-bold ">{item.name}</span>
        <span class="text-slate-200 font-thin">{item.post}</span>
      </div>
    </li>
    {/each}
  </ul>
</div>

<style>
    @import './global.css';
.custom-border{
  border-bottom-width:0.005px;
  border-color: #2b2b2b
}
</style>

