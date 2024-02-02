<script lang="ts">
    export let title: string;
    export let content: string;
    export let link: string;
    export let gitLink: string;

</script>

<a href="projects/{link}">
<div class= "relative bg-gray-50 h-1/5 w-full px-5 py-5 mx-auto my-5 border-l-2 border-b-2 border-gray-200 rounded-lg shadow card-pulse text-left">
    <!-- Header for card -->
    <div>
        <h1 class="text-gray-600 text-3xl font-bold py-2">{title}</h1>
        <hr class="py-1">
    </div>
    <!-- Post description? for card -->
    <div>    
    <p class="text-gray-500">{content}</p>
    </div>
    <!-- Footer for card -->
    <div class="absolute bottom-5">
    <hr class="py-1">
    <a class="underline text-gray-400" href={gitLink}>{gitLink}</a>
    </div>
</div>
</a>

<style lang="postcss">
    .card-pulse:hover{
        animation: pulse-animation 1s infinite;
    }

    @keyframes pulse-animation{
        0% {
            box-shadow: 0 0 0 0px rgba(0, 0, 0, 0.1);
        }

        100% {
            box-shadow: 0 0 0 10px rgba(0, 0, 0, 0);
        }
    }
</style>