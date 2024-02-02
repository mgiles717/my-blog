<script lang="ts">
    import Sidebar from "../../components/Sidebar.svelte";
</script>

<div class="flex">
    <Sidebar/>
    <main class="fade-in flex-1 flex-col text-center">
        <div class="justify-center">
            <img class="w-full mx-auto" src="/images/graduation.jpg" alt="My Graduation">
            <h1 class="px-6 py-4 text-5xl text-gray-400 font-bold text-left">About me</h1>
            <p class="px-6 pt-4 text-gray-800 font-semibold text-left">The picture above is me! I graduated from UEA with a First Class Masters of Computing (MComp), this means I learnt how to build funny websites like this. I spent a glorious 5 years due to taking a foundation year as well, and had the opportunity to mature and develop my understanding of such a fascinating and broad field.</p>
            <p class="px-6 pt-4 text-gray-800 font-semibold text-left">I have since developed a great interest in machine learning, data science, artificial intelligence, bioinformatics and cyber security to name a few. A friend and I read a lot of machine learning papers during my Masters year whilst ChatGPT was taking the world by storm, and we both loved seeing the transformer and LLM revolution unfold.</p>
            <p class="px-6 pt-4 text-gray-800 font-semibold text-left">I want to use my skills and understanding to make a difference in the world, to do some good which is in great demand at the moment. I hope to pursue a career in a data related field to create stories and meaningful insights from otherwise complex and convoluted data.</p>
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