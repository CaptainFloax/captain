<script setup lang="ts">
    import ButtonParticle from '../../particles/button/ButtonParticle.vue';
    const menuItems: {name: string, link:string}[] = [
        {
            'name': 'Ressources',
            'link': '/ressources'
        },
        {
            'name': 'Services',
            'link': '/services'
        },
        {
            'name': 'Portfolio',
            'link': '/porfolio'
        },
        {
            'name': 'A propos',
            'link': '/about'
        },
        {
            'name': 'Contact',
            'link': '/contact'
        },
    ]
</script>

<template>
    <header>
        <div class="classic-container">
            <div class="menu">
                <div class="m-logo">
                    <img src="src/assets/img/branding/logo.svg" />
                </div>
                <ul class="m-items">
                    <li class="mi-item" v-for="(item, index) in menuItems" :key="index">
                        <a :href="item.name">{{ item.name }}</a>
                    </li>
                </ul>
            </div>
            <div class="actions">
                <ButtonParticle level="2" color="primary" label="Travailler avec nous"/>
            </div>
        </div>
    </header>
</template>

<style lang="scss">
    @use './HeaderComponent';
</style>