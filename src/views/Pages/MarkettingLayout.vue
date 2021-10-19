<template>
  <div class="wrapper">
    <b-navbar toggleable="lg" class="navbar-horizontal">
      <b-navbar-brand href="#"
        >Nanna Mane -
        <p>We serve all your real esate needs</p></b-navbar-brand
      >

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <base-header class="pb-1 pb-1 pt-1 pt-md-1 bg-gradient-info">
        <b-card>
          <b-media no-body class="align-items-center">
            <span class="avatar avatar-sm">
              <b-img
                alt="Image placeholder"
                rounded="circle"
                src="img/kashif.png"
              />
            </span>
            <b-media-body class="ml-2 d-none d-lg-block">
              <span class="mb-0 text-sm  font-weight-bold">Kashif</span>
            </b-media-body>
          </b-media>
          <b-card-text class="mb-0 text-sm  font-weight-bold">
            <i class="ni ni-headphones "></i>
            9686496343
          </b-card-text>
          <b-card-text class="mb-0 text-sm  font-weight-bold">
            <i class="ni ni-email-83"></i>
            info@nannamane.com
          </b-card-text>
        </b-card>
      </base-header>
      <base-header class="pb-1 pb-1 pt-1 pt-md-1 bg-gradient-info">
        <b-card>
          <b-media no-body class="align-items-center">
            <span class="avatar avatar-sm">
              <b-avatar />
            </span>
            <b-media-body class="ml-2 d-none d-lg-block">
              <span class="mb-0 text-sm  font-weight-bold">Mustafa</span>
            </b-media-body>
          </b-media>
          <b-card-text class="mb-0 text-sm  font-weight-bold">
            <i class="ni ni-headphones "></i>
            8431796515
          </b-card-text>
          <b-card-text class="mb-0 text-sm  font-weight-bold">
            <i class="ni ni-email-83"></i>
            info@nannamane.com
          </b-card-text>
        </b-card>
      </base-header>
      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-form>
            <b-nav-item-dropdown right>
              <template v-slot:button-content>
                <i class="ni ni-settings-gear-65"></i>
                <span class="nav-link-inner--text d-lg-none">Settings</span>
              </template>
              <b-dropdown-item href="/#/dashboard">Product</b-dropdown-item>
            </b-nav-item-dropdown>
          </b-nav-form>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>

    <b-carousel
      id="carousel"
      controls
      indicators
      img-width="1024"
      img-height="300"
      :interval="2000"
    >
      <b-carousel-slide
        text="Nanna mane helps you get your dream home : please contact info@nannamane.com"
        img-src="img/home.jpg"
      ></b-carousel-slide>
      <b-carousel-slide
        text="Nanna mane helps you get your dream estate : please contact info@nannamane.com"
        img-src="img/estate.jpeg"
      ></b-carousel-slide>
      <b-carousel-slide
        text="Looking for a plot in your budget  : please contact info@nannamane.com"
        img-src="img/site.jpeg"
      ></b-carousel-slide>
    </b-carousel>
    <base-header class="pb-6 pb-8 pt-4 pt-md-4 bg-gradient-success">
      <b-card-header>
        <b-card-text>
          Premium Properties - Verified
        </b-card-text></b-card-header
      >
      <!-- Card stats -->
      <b-card-group deck class="pb-6 pb-8 pt-4 pt-md-4 bg-gradient-success">
        <b-card
          title="Card Title"
          img-src="img/site.jpeg"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2"
        >
          <b-card-text>
            30x40 site in Hassan
          </b-card-text>

          <small class="text-muted">Last updated 3 mins ago</small>
        </b-card>
        <b-card
          title="Card Title"
          img-src="img/estate.jpeg"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2"
        >
          <b-card-text>
            Estate in madikere
          </b-card-text>

          <small class="text-muted">Last updated 3 mins ago</small>
        </b-card>
      </b-card-group>
    </base-header>
  </div>
</template>
<script>
export default {
  data() {
    return {
      model: {
        email: "",
        password: "",
        rememberMe: false
      }
    };
  },
  methods: {
    onSubmit() {
      // this will be called only after form is valid. You can do api call here to login
    }
  }
};
</script>
