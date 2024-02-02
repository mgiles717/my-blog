<script lang="ts">
    import Sidebar from "../../components/Sidebar.svelte";
</script>

<div class="flex">
    <Sidebar/>
    <main class="fade-in flex-1 flex-col text-center">
        <div class="h-screen flex items-center justify-center">
            <div class="text-center">
        <h1 class="px-6 text-5xl text-gray-400 font-bold text-left">Work in progress!</h1>
        <p class="px-6 pt-4 text-gray-800 font-semibold text-left">I'm currently working on this page, come back later!.
        </div>
    </div>
        </main>
</div>

<style lang="postcss">
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