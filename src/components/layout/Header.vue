<script setup>
import Button from '../../components/basic/Button.vue'

const clickServices = () => {
  console.log('click Services');
};

const clickCall = () => {
    console.log('click Book a Call');
}
</script>

<template>
    <header class="container">
        <div class="header-wrap">
            <div class="logo">
                <img alt="a-consult logo" src="@/assets/img/logo.png" />
            </div>
            <div class="nav">
                <Button @click="clickServices">Services</Button>
                <Button @click="clickCall" type="blue">
                    <template #icon>
                        <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M18.3472 13.3556L13.9306 11.3766L13.9184 11.3709C13.6892 11.2729 13.439 11.2335 13.1907 11.2564C12.9424 11.2793 12.7037 11.3638 12.4963 11.5022C12.4718 11.5183 12.4484 11.5358 12.4259 11.5547L10.1441 13.5C8.69845 12.7978 7.20595 11.3166 6.50376 9.88968L8.45188 7.57312C8.47063 7.54968 8.48845 7.52624 8.50532 7.50093C8.64072 7.29403 8.72287 7.05686 8.74446 6.81053C8.76605 6.5642 8.72641 6.31636 8.62907 6.08906V6.07781L6.64438 1.65374C6.5157 1.3568 6.29444 1.10944 6.01362 0.948592C5.7328 0.787739 5.4075 0.722019 5.08626 0.761243C3.81592 0.928406 2.64986 1.55228 1.80588 2.51633C0.961903 3.48039 0.497712 4.7187 0.500008 5.99999C0.500008 13.4437 6.55626 19.5 14 19.5C15.2813 19.5023 16.5196 19.0381 17.4837 18.1941C18.4477 17.3501 19.0716 16.1841 19.2388 14.9137C19.2781 14.5926 19.2125 14.2674 19.0518 13.9866C18.8911 13.7058 18.644 13.4845 18.3472 13.3556ZM14 18C10.8185 17.9965 7.76825 16.7311 5.51856 14.4814C3.26888 12.2318 2.00348 9.18152 2.00001 5.99999C1.99648 5.08451 2.32631 4.19905 2.92789 3.50897C3.52947 2.81888 4.36167 2.37137 5.26907 2.24999C5.2687 2.25373 5.2687 2.2575 5.26907 2.26124L7.23782 6.66749L5.30001 8.98687C5.28034 9.0095 5.26247 9.03364 5.24657 9.05906C5.10549 9.27554 5.02273 9.5248 5.0063 9.78268C4.98988 10.0406 5.04035 10.2983 5.15282 10.5309C6.0022 12.2681 7.75251 14.0053 9.50845 14.8537C9.74279 14.9652 10.002 15.0139 10.2608 14.9952C10.5196 14.9764 10.7692 14.8909 10.985 14.7469C11.0091 14.7307 11.0322 14.7131 11.0544 14.6944L13.3334 12.75L17.7397 14.7234C17.7397 14.7234 17.7472 14.7234 17.75 14.7234C17.6301 15.6321 17.1833 16.466 16.4931 17.0691C15.8028 17.6721 14.9166 18.0031 14 18Z" fill="white"/>
                        </svg>
                    </template>
                    Book a Call
                </Button>
            </div>
        </div>
    </header>
</template>

<style scoped>
.header-wrap {
    display: flex;
    justify-content: space-between;
    padding: 16px;
}

.logo {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-left: 108px;
}
.nav {
    width: 440px;
    display: flex;
    justify-content: space-between;
}
</style>