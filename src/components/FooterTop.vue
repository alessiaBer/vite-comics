<script>
export default {
    name: 'FooterTop',
    data() {
    return {
        menu: [
        {
            title: 'DC Comics',
            items: [
                'Characters',
                'Comics',
                'Movies',
                'TV',
                'Games',
                'Videos',
                'News'
            ]
        },
        {
            title: 'DC',
            items: [
                'Terms of Use',
                'Privacy Policy (New)',
                'Ad Choice',
                'Avertising',
                'Jobs',
                'Subscriptions',
                'Talent Workshop',
                'CPSC Certificates',
                'Ratings',
                'Shop Help',
                'Contact Us'
            ]
        },
        {
            title: 'Sites',
            items: [
                'DC',
                'MAD Magazine',
                'DC Kids',
                'DC Universe',
                'DC Power Visa'
            ]
        },
        {
            title: 'Shop',
            items: [
                'Shop DC',
                'Shop DC Collectibles'
            ] 
        }
    ]
    };
  },
};
</script>
<template>
  <div class="footer_top">
      <div class="top_container">
        <div class="footer_menu">
            <div class="my_col" v-for="list in menu">
                <h5>{{ list.title.toUpperCase() }}</h5>
                <ul class="list-unstyled">
                    <li v-for="item in list.items">
                        <a href="#">{{ item }}</a>
                    </li>
                </ul>
            </div>
        </div>
        <div class="footer_logo">
        </div>

      </div>
    </div>
</template>

<style lang="scss" scoped></style>
