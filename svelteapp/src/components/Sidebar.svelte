<script lang="ts">
    export let width = "w-1/3";

    let asset_path: string = '/images/'
    const sidebarImage: string = asset_path + 'sidebarImage.jpg'
    const githubIcon: string =  asset_path + 'github.svg'
    const linkedinIcon: string = asset_path + 'linkedin.svg'
</script>

<div class="h-screen bg-gray-100 {width} border-r border-gray-300 flex flex-col items-center justify-center">
    <div class="flex items-center justify-center">
        <a class="w-10/12 mx-auto" href="/"><img class="rounded-full drop-shadow-lg hover:sepia" src="{sidebarImage}" alt="me :)"></a>
    </div>
    <div class="flex items-center justify-center h-14"> 
    <h1 class="text-gray-800 text-3xl font-semibold text-center">Max Giles</h1>
    </div>
    <div class="flex items-center justify-center">
        <h3 class="text-gray-500 text-xl text-center"> Aspiring Bioinformatician </h3>
    </div>
    <nav class="flex flex-col items-center justify-between hfull">
        <ul class="py-4 justify-center inline-flex border-b border-gray-300">
            <li class="mx-auto px-3"><a href="about" class="text-gray-400 hover:text-slate-700">About</a></li>
            <li class="mx-auto px-3"><a href="portfolio" class="text-gray-400 hover:text-slate-700">Portfolio</a></li>
            <li class="mx-auto px-3"><a href="blog" class="text-gray-400 hover:text-slate-700">Blog</a></li>
        </ul>
    </nav>
    <div class="flex items-center justify-center">
        <ul class="py-4 justify-center inline-flex"> 
            <li class="mx-auto px-3"><a href="https://github.com/mgiles717"><img class="h-8 hover-shake" src="{githubIcon}" alt="Github"></a></li>
            <li class="mx-auto px-3"><a href="https://www.linkedin.com/in/mgiles717/"><img class="h-8 hover-shake" src="{linkedinIcon}" alt="LinkedIn"></a></li>
        </ul>
    </div>
</div>

<style lang="postcss">
    .hover-shake:hover{
        animation: shake 0.5s;
        animation-iteration-count: infinite;
    }

    @keyframes shake {
        0% { transform: translate(1px, 1px) rotate(0deg); }
        10% { transform: translate(-1px, -2px) rotate(-1deg); }
        20% { transform: translate(-3px, 0px) rotate(1deg); }
        30% { transform: translate(3px, 2px) rotate(0deg); }
        40% { transform: translate(1px, -1px) rotate(1deg); }
        50% { transform: translate(-1px, 2px) rotate(-1deg); }
        60% { transform: translate(-3px, 1px) rotate(0deg); }
        70% { transform: translate(3px, 1px) rotate(-1deg); }
        80% { transform: translate(-1px, -1px) rotate(1deg); }
        90% { transform: translate(1px, 2px) rotate(0deg); }
        100% { transform: translate(1px, -2px) rotate(-1deg); }
    }
</style>