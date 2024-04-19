<script setup>
// const team = [
//     {
//         name: 'Thomas Lundberg',
//         position: 'A-consult Co-owner',
//         img: '/src/assets/img/thomas-lundberg.jpg'
//     },
//     {
//         name: 'Ivan Nikolaichuk',
//         position: 'A-consult Co-owner',
//         img: '/assets/img/ivan-nikolaichuk.jpg',
//     },
//     {
//         name: 'Allan Green',
//         position: 'Software Developer',
//         img: '/assets/img/allan-green.jpg',
//     },
//     {
//         name: 'Matt Piers',
//         position: 'Head of Marketing',
//         img: '/assets/img/matt-piers.jpg',
//     }
// ]
</script>

<template>
<div class="team">
    <div class="container">
        <div class="title">Meet our team</div>
        <div class="team-list">
            <!-- <div class="team-item" v-for="(item, index) in team" :key="'team-member-' + index">
                <div class="team-img"><img :alt="'Team member ' + item.name + ' photo'" :src="item.img" /></div>
                <div class="team-name"> {{ item.name }} </div>
                <div class="team-position"> {{ item.position }} </div>
            </div> -->
            <div class="team-item">
                <div class="team-img"><img alt="thomas lundberg photo" src="@/assets/img/thomas-lundberg.jpg" /></div>
                <div class="team-name">Thomas Lundberg</div>
                <div class="team-position">A-consult Co-owner</div>
            </div>
            <div class="team-item">
                <div class="team-img"><img alt="ivan nikolaichuk photo" src="@/assets/img/ivan-nikolaichuk.jpg" /></div>
                <div class="team-name">Ivan Nikolaichuk</div>
                <div class="team-position">A-consult Co-owner</div>
            </div>
            <div class="team-item">
                <div class="team-img"><img alt="allan green photo" src="@/assets/img/allan-green.jpg" /></div>
                <div class="team-name">Allan Green</div>
                <div class="team-position">Software Developer</div>
            </div>
            <div class="team-item">
                <div class="team-img"><img alt="matt piers photo" src="@/assets/img/matt-piers.jpg" /></div>
                <div class="team-name">Matt Piers</div>
                <div class="team-position">Head of Marketing</div>
            </div>
        </div>
    </div>
</div>
</template>

<style scoped>
.team {
    padding: 65px 0;
    background-color: var(--gray-10);
}
.team-list {
    display: flex;
    justify-content: space-between;
    margin-top: 46px;
}
.team-name {
    color: var(--blue-500);
}
.team-position {
    color: var(--blue-200);
    font-size: 14px;
    font-weight: 400;
}
</style>