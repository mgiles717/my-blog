<script lang="ts">
    import Sidebar from "../../components/Sidebar.svelte";
    import ProjectCard from "../../components/Card/ProjectCard.svelte";

</script>

<div class="flex">
    <Sidebar/>
    <main class="fade-in flex-1 flex-col text-center">
        <div class="h-screen flex justify-center">
            <div class="text-center w-4/5">
                <ProjectCard title="This blog!" content="Creating a website using Svelte is enjoyable, it won't convert me to a fully fledged web developer though. My first meaningful step to highlighting my projects was through developing this website. I liked to keep the style minimalistic as possible while maintaining aesthetics." link="theBlog" gitLink="https://github.com/mgiles717/my-blog"></ProjectCard>
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