<script setup>
import FAQItem from '../components/FAQItem.vue'
import Button from '../components/basic/Button.vue'

const questions = [
    {
        title: 'What services does your company offer?',
        text: 'We offer a wide range of IT consulting services, including IT strategy development, digital transformation, cybersecurity, cloud solutions, and more. Our expertise will help your business adapt, grow, and stand out in the market.',
    },
    {
        title: 'How do you ensure the security of my data?',
        text: 'We adhere to strict security standards and implement advanced technologies to protect your data. Our cybersecurity solutions provide reliable protection against threats and external attacks while complying with all regulatory requirements.',
    },
    {
        title: 'What is your experience working with my industry?',
        text: 'Our specialists have extensive experience working across various industries, including finance, healthcare, retail, and many more. We develop tailored IT solutions, considering the specifics of your industry and business objectives.',
    },
    {
        title: 'What are your pricing and payment structure?',
        text: 'We offer a flexible pricing policy and payment structure tailored to the needs and budget of your business. The cost of services depends on the scope of work, project complexity, and the chosen service package. We are always ready to provide a detailed commercial proposal upon your request.',
    },
    {
        title: 'How can I start collaborating with your company?',
        text: 'To start collaborating with us, simply contact our team through the contact form on the website, send an email to the provided address, or call the listed phone numbers. Our specialist will discuss your needs, goals, and offer optimal solutions for your business.',
    },    
]

const clickCall = () => {
    console.log('Contact Now')
};

</script>

<template>
<div class="faq">
    <div class="faq-wrap container">
        <div class="faq-content">
            <div class="faq-title title">Frequently Asked Questions</div>
            <div class="faq-subtitle">Your IT Consulting Queries Answered</div>
            <div class="faq-list">
                <FAQItem v-for="(item, index) in questions" :key="'question-' + index"
                    :title="item.title"
                    :text="item.text"
                >  
                </FAQItem>
            </div>
        </div>
        <div class="faq-contact">
            <div class="faq-contact-icon">
                <svg width="118" height="118" viewBox="0 0 118 118" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <g clip-path="url(#clip0_24_3458)">
                    <path d="M75.4256 37.1128C80.9535 37.4133 86.3162 39.1036 91.0173 42.0273C95.7184 44.9509 99.6059 49.0134 102.32 53.8385C105.034 58.6637 106.487 64.0955 106.544 69.6313C106.601 75.1671 105.26 80.6278 102.646 85.5078L106.376 98.195C106.561 98.825 106.573 99.4932 106.41 100.129C106.248 100.766 105.917 101.346 105.453 101.811C104.989 102.275 104.408 102.606 103.772 102.768C103.136 102.93 102.467 102.918 101.837 102.733L89.164 98.9902C84.9775 101.229 80.3564 102.536 75.6175 102.822C70.8785 103.108 66.1338 102.366 61.7086 100.646C57.2833 98.9268 53.2822 96.2708 49.9795 92.8603C46.6769 89.4498 44.1507 85.3654 42.5742 80.8872" fill="#CEEEFF"/>
                    <path d="M15.3538 63.5704C11.6292 56.6122 10.5296 48.5471 12.2554 40.8458C13.9812 33.1444 18.4174 26.3199 24.7552 21.6166C31.093 16.9132 38.9101 14.6444 46.7812 15.2239C54.6522 15.8033 62.0528 19.1924 67.6335 24.7731C73.2142 30.3538 76.6033 37.7544 77.1827 45.6254C77.7622 53.4965 75.4934 61.3136 70.79 67.6514C66.0867 73.9892 59.2621 78.4254 51.5608 80.1512C43.8595 81.877 35.7944 80.7774 28.8362 77.0528L16.149 80.7822C15.519 80.9672 14.8508 80.9792 14.2146 80.8168C13.5784 80.6544 12.9977 80.3237 12.5334 79.8595C12.0692 79.3952 11.7385 78.8144 11.5761 78.1782C11.4137 77.542 11.4257 76.8739 11.6107 76.2439L15.3538 63.5704Z" fill="#064163"/>
                    </g>
                    <defs>
                    <clipPath id="clip0_24_3458">
                    <rect width="117" height="117" fill="white" transform="translate(0.5 0.5)"/>
                    </clipPath>
                    </defs>
                </svg>
            </div>
            <div class="faq-contact-title">Still Have Questions?</div>
            <div class="faq-contact-text">Feel free to reach out to us. Our team is here to provide you with all the answers you need to make informed decisions about your IT consulting needs.</div>
            <Button class="faq-contact-call-btn" @click="clickCall" type="blue">
                <template #icon>
                    <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M18.3472 13.3556L13.9306 11.3766L13.9184 11.3709C13.6892 11.2729 13.439 11.2335 13.1907 11.2564C12.9424 11.2793 12.7037 11.3638 12.4963 11.5022C12.4718 11.5183 12.4484 11.5358 12.4259 11.5547L10.1441 13.5C8.69845 12.7978 7.20595 11.3166 6.50376 9.88968L8.45188 7.57312C8.47063 7.54968 8.48845 7.52624 8.50532 7.50093C8.64072 7.29403 8.72287 7.05686 8.74446 6.81053C8.76605 6.5642 8.72641 6.31636 8.62907 6.08906V6.07781L6.64438 1.65374C6.5157 1.3568 6.29444 1.10944 6.01362 0.948592C5.7328 0.787739 5.4075 0.722019 5.08626 0.761243C3.81592 0.928406 2.64986 1.55228 1.80588 2.51633C0.961903 3.48039 0.497712 4.7187 0.500008 5.99999C0.500008 13.4437 6.55626 19.5 14 19.5C15.2813 19.5023 16.5196 19.0381 17.4837 18.1941C18.4477 17.3501 19.0716 16.1841 19.2388 14.9137C19.2781 14.5926 19.2125 14.2674 19.0518 13.9866C18.8911 13.7058 18.644 13.4845 18.3472 13.3556ZM14 18C10.8185 17.9965 7.76825 16.7311 5.51856 14.4814C3.26888 12.2318 2.00348 9.18152 2.00001 5.99999C1.99648 5.08451 2.32631 4.19905 2.92789 3.50897C3.52947 2.81888 4.36167 2.37137 5.26907 2.24999C5.2687 2.25373 5.2687 2.2575 5.26907 2.26124L7.23782 6.66749L5.30001 8.98687C5.28034 9.0095 5.26247 9.03364 5.24657 9.05906C5.10549 9.27554 5.02273 9.5248 5.0063 9.78268C4.98988 10.0406 5.04035 10.2983 5.15282 10.5309C6.0022 12.2681 7.75251 14.0053 9.50845 14.8537C9.74279 14.9652 10.002 15.0139 10.2608 14.9952C10.5196 14.9764 10.7692 14.8909 10.985 14.7469C11.0091 14.7307 11.0322 14.7131 11.0544 14.6944L13.3334 12.75L17.7397 14.7234C17.7397 14.7234 17.7472 14.7234 17.75 14.7234C17.6301 15.6321 17.1833 16.466 16.4931 17.0691C15.8028 17.6721 14.9166 18.0031 14 18Z" fill="white"/>
                    </svg>
                </template>
                Contact Now
            </Button>
        </div>
    </div>
</div>
</template>

<style scoped>
.faq {
    margin-left: 140px;
    padding: 15px 0;
}
.faq-wrap {
    display: flex;
    /* justify-content: space-between; */
}
.faq-content {
    width: 604px;
}
.faq-title {
    text-align: left;
}
.faq-subtitle {
    color: var(--blue-500);
    font-size: 20px;
}
.faq-list {
    margin-top: 84px;
}
.faq-contact {
    position: relative;
    width: 412px;
    height: 386px;
    margin-top: 175px;
    margin-left: 125px;
    padding: 15px 30px;
    background-color: var(--gray-10);
    border-radius: 10px;
    border: 2px solid var(--gray-40);
}
.faq-contact::after {
    content: '';
    position: absolute;
    width: 630px;
    height: 646px;
    top: -65%;
    left: 4%;
    background-image: url('/src/assets/img/circles-2.png');
    z-index: -1;
}
.faq-contact-icon {
    width: 118px;
    margin: 0 auto;
}
.faq-contact-title {
    margin-top: 6px;
    color: var(--blue-700);
    font-size: 18px;
    text-align: center;
}
.faq-contact-text {
    margin-top: 8px;
    color: var(--blue-300);
    font-size: 14px;
    line-height: 1.7;
    font-weight: 400;
    text-align: center;
}
.faq-contact-call-btn {
    margin: 25px auto 0 auto;
}
</style>