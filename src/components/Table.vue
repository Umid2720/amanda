<template>
    <div class="table">
        <table width="100%">
            <thead width="100%">
                <tr>
                    <td>
                        <label>
                            <input type="checkbox">
                        </label>
                    </td>
                    <td>Email</td>
                    <td>Sent</td>
                    <td>Date</td>
                    <td>Open</td>
                    <td>Click</td>
                    <td>Bounce</td>
                    <td>Unsub.</td>
                    <td>Status</td>
                </tr>
            </thead>
            <tbody>
                <tr class="" v-for="l in 10" :key="l">
                    <td><label><input type="checkbox"></label></td>
                    <td class="flex items-center"><img src="../assets/gallery.svg" alt="gallery">Discount 20% OFF</td>
                    <td>6.98K</td>
                    <td>01/09/22</td>
                    <td>2.09%</td>
                    <td>1.05%</td>
                    <td>0.07%</td>
                    <td>-</td>
                    <td>Draft</td>
                </tr>
            </tbody>
        </table>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.table {
    margin-top: 24px;
    border-radius: 8px;
    padding: 26px 35px 0 26px;
    border: 1px solid #EAEAEA;
}

.table thead {
    margin-bottom: 40px;
}
</style>