<template>
    <main class="main">
        <header class="header flex items-center justify-between">
            <div class="header__title">
                <h3>Welcome, Amanda</h3>
                <div class="header__date">Tue, 07 June 2022</div>
            </div>
            <div class="header__left flex">
                <Search />
                <button>
                    <img src="../assets/bing.svg" alt="bing">
                </button>
                <img src="../assets/avatar.png" alt="avatar">
            </div>
        </header>
        <h3 class="project__title">
            Email Marketing
        </h3>
        <div class="flex justify-between main__lists">
            <Sari sariTitle="Set" sariResult="12.6K" />
            <Sari sariTitle="Open" sariResult="25.1%" />
            <Sari sariTitle="Unsubscribe" sariResult="1.98%" />
            <Sari sariTitle="Sales" sariResult="16.04%" />
            <Sari sariTitle="Click" sariResult="3.98%" />
            <Sari sariTitle="Bounce" sariResult="2.09%" />
        </div>
        <div class="flex justify-between">
            <div class="main__buttons">
                <Button>All</Button>
                <Button>Draft</Button>
                <Button>Sent</Button>
                <Button>Scheduled</Button>
            </div>
            <Search />
        </div>
        <Table />
    </main>
</template>

<script>
import Sari from './Sari.vue'
import Table from './Table.vue'
import Search from './Search.vue'
import Button from './Button.vue'
export default {
    components: { Search, Sari, Button, Table },
}
</script>

<style>
.main {
    flex: 1;
    padding: 32px 40px 0;
}

.header__title h3 {
    font-size: 24px;
    font-weight: 500;
    margin-bottom: 16px;
}

.header__date {
    line-height: 21px;
    color: var(--A2Color);
}

.header__left {
    column-gap: 20px;
}

.header__left label {
    width: 400px;
}

.header__left button {
    padding: 12px;
    border-radius: 10px;
    border: 1px solid var(--EColor);
}

.project__title {
    font-size: 20px;
    font-weight: 500;
    line-height: 26px;
    margin: 32px 0 24px;
}

.main__buttons {
    margin-right: 20px;
}

.main__buttons button:not(:last-child) {
    margin-right: 20px;
}

.main__lists {
    margin-bottom: 32px;
}

.main .search label {
    width: 400px;
}
</style>