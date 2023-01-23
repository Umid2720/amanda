<template>
    <aside class="sidebar flex">
        <button class="sidebar__button block">
            <img src="../assets/gallery.svg" alt="galery.png">
        </button>
        <Search />
        <p class="sidebar__title">Menu</p>
        <ul class="sidebar__menu">
            <li class="sidebar__menu-item" v-for="(pic, id) in pictures" :key="id">
                <a href="" class="sidebar__link flex">
                    <img :src="'/src/assets/' + pic + '.svg'" :alt="pic">
                    {{ pic }}
                </a>
            </li>
        </ul>

        <div class="sidebar__bottom">
            <p class="sidebar__title">Profile</p>
            <div class="sidebar__profile flex items-center justify-between">
                <img src="../assets/amanda.png" alt="">
                <div class="sidebar__profile-name">
                    <h4 class="sidebar__profile-avatar">Amanda</h4>
                    <p class="admin">Admin Account</p>
                </div>
                <button class="sidebar__profile-property flex">
                    <span></span>
                    <span></span>
                    <span></span>
                </button>
            </div>
            <button class="logout flex">
                <img src="../assets/logout.svg" alt="logout">
                Logout
            </button>
        </div>
    </aside>
</template>

<script>
import Search from './Search.vue'
export default {
    components: { Search },
    data() {
        return {
            pictures: ['overview', 'product', 'marketing', 'sales', 'cloud', 'settings']
        }
    }
}

</script>

<style>
.sidebar {
    padding: 32px;
    height: 100vh;
    max-width: 320px;
    flex-direction: column;
    border-right: 1px solid var(--EColor);
}

.sidebar__button {
    padding: 16px 83px;
    margin: 0 auto 16px;
    background-color: var(--bodyColor);
}

.sidebar__title {
    color: var(--BColor);
    font-size: 14px;
    font-weight: 500;
    margin-top: 40px;
    line-height: 18px;
    margin-bottom: 20px;
}

.sidebar__menu-item:not(:last-child) {
    margin-bottom: 30px;
}

.sidebar__link {
    column-gap: 24px;
    line-height: 21px;
    color: var(--BColor);
    text-transform: capitalize;
}

.sidebar__link:hover {
    color: var(--purple);
}

.sidebar__bottom {
    margin-top: auto;
}

.sidebar__profile-avatar {
    font-weight: 500;
    line-height: 21px;
}

.admin {
    font-size: 14px;
    margin-top: 10px;
    color: var(--AColor);
}

.sidebar__profile-property {
    column-gap: 3.75px;
}

.sidebar__profile-property span {
    width: 2.25px;
    height: 2.25px;
    border-radius: 50%;
    background-color: var(--AColor);
}

.logout {
    width: 100%;
    color: var(--white);
    font-size: 16px;
    margin-top: 40px;
    line-height: 24px;
    padding: 14px 22px;
    font-family: 'Poppins';
    background-color: var(--purple);
}

.logout img {
    margin-right: 16px;
}
</style>