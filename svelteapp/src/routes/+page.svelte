<script lang="ts">
    import Sidebar from "../components/Sidebar.svelte";
</script>

<div class="flex">
    <Sidebar/>
    <main class="fade-in flex-1 flex-col text-center">
        <div class="h-screen flex items-center justify-center">
            <div class="text-center">
        <h1 class="px-6 text-5xl text-gray-400 font-bold text-left">Welcome to my website!</h1>
        <p class="px-6 pt-4 text-gray-800 font-semibold text-left">I am a MComp Computing Sciences graduate, my interests lie in machine learning, bioinformatics, structural and computational biology and cyber security. You can check out my projects I've worked on <a class="font-bold hover:text-gray-600" href="portfolio">here</a>.</p>
        <p class="px-6 pt-4 text-gray-800 font-semibold text-left">In my spare time, I love to play video games such as DOTA 2, rave about music like The Smashing Pumpkins and Queens of The Stone Age and lastly I love to play guitar and sing as bad as I am. I try to keep my interests broad as possible.</p>
        </div>
    </div>
        </main>
</div>

<style>
    @keyframes fade-in{
        0% {
            opacity: 0;
            transform: translateY(20%);
            /* transform: translateX(0); */
        }
        100% {
            opacity: 1;
            transform: translateY(0);
            /* transform: translateX(0); */
        }
    }

    .fade-in{
        animation-name: fade-in;
        animation-duration: 1s;
    }
</style>
