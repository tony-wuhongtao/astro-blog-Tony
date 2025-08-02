<script lang="ts">
    import kwesforms from 'kwesforms';  
    import {onMount} from 'svelte';

    onMount(() => {

        kwesforms.init();

    });
</script>

<form method="POST" action="https://kwesforms.com/api/f/K5ar2WuGVs26ym4O3DYb" class="kf-form grid gap-y-2"
    no-error-message
    redirect="/thankyou">

    <label for="comment" class="text-zinc-900 text-2xl mb-2 mt-10">
        What's on your mind?
    </label>
    <textarea class="border border-teal-900 rounded-lg text-2xl px-6 py-6"
    name="comment" id="comment" rows="3"  
    rules="required|max:255" >

    </textarea>
    <button type="submit" class="text-2xl text-zinc-100 bg-teal-900 px-6 py-5 rounded-xl my-1 cursor-pointer hover:bg-teal-600">
        Send
    </button>

</form>  