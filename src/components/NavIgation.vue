<template>
    <nav>
        <a class="menu" href="#" @click.prevent="fix(1)" ref="act1">O mnie</a>
        <a class="menu" href="#" @click.prevent="fix(2)" ref="act2">Aktualność</a>
        <a class="menu" href="#" @click.prevent="fix(3)" ref="act3">Hobby</a>
        <a class="menu" href="#" @click.prevent="fix(4)" ref="act4">Kontakt</a>
    </nav>
</template>

<script>
export default {
    data() {
        return {
            activeLink: null
        };
    },
    methods: {
        fix(x) {
            this.activeLink = x;
            this.updateActiveClass();
        },
        updateActiveClass() {
            this.$refs.act1.classList.remove('active');
            this.$refs.act2.classList.remove('active');
            this.$refs.act3.classList.remove('active');
            this.$refs.act4.classList.remove('active');

            if (this.activeLink === 1) {
                this.$refs.act1.classList.add('active');
            } else if (this.activeLink === 2) {
                this.$refs.act2.classList.add('active');
            } else if (this.activeLink === 3) {
                this.$refs.act3.classList.add('active');
            } else if (this.activeLink === 4) {
                this.$refs.act4.classList.add('active');
            }
        }
    }
};
</script>

<style>
nav {
    background-color: darkcyan;
    overflow: hidden;
}
nav a {
    display: inline-block;
    width: 15%;
    padding: 15px 30px;
    color: white;
    text-align: center;
    text-decoration: none;
}
nav a:hover {
    color: crimson;
    background-color: white;
}
.active {
    background-color: crimson;
}
</style>
