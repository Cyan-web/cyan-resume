<div>
    <div class="flex flex-col justify-center items-center text-center">
        <img
            alt="avatar"
            class="w-20 rounded-full"
            src="https://avatars.githubusercontent.com/u/45061152?v=4"
        >

        <h2 class="mt-2 text-xl font-medium">
            Cyan
        </h2>
    </div>

    <div class="w-max mx-auto">
        <h4 class="text-center">
            前端基础技能
        </h4>

        <div class="">
            {#each skills as { title, icon } (title)}
                <Skill icon={icon} title={title} />
            {/each}
        </div>

        <h4 class="text-center">
            框架掌握
        </h4>

        <div class="">
            {#each frameworks as { title, icon } (title)}
                <Skill icon={icon} title={title} />
            {/each}
        </div>
    </div>
</div>

<script>
    import Skill from './Skill.svelte'

    const skills = [
        {
            title: 'HTML',
            icon: 'icon-HTML1'
        },
        {
            title: 'CSS',
            icon: 'icon-CSS2'
        },
        {
            title: 'JavaScript',
            icon: 'icon-JavaScript'
        },
        {
            title: 'TypeScript',
            icon: 'icon-typescript'
        }
    ]

    const frameworks = [
        {
            title: 'Vue2.x',
            icon: 'icon-Vue'
        },
        {
            title: 'Vue3.x',
            icon: 'icon-Vue'
        },
        {
            title: 'React',
            icon: 'icon-React'
        }
    ]
</script>
