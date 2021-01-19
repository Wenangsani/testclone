<script>
  import { onMount } from "svelte";
  import NavbarGuest from "../component/navbar_guest.svelte";
  import Footer from "../component/footer.svelte";

  let listClass = [
    {
      pict:
        "https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/categories/Mobile_Category_Yoga.jpg",
      name: "YOGA",
      desc: "From Ashtanga to Vinyasa, make mindful movement a daily ritual.",
    },
    {
      pict:
        "https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/categories/Mobile_Category_Fitness.jpg",
      name: "FITNESS",
      desc:
        "Train on your time with Strength, Barre, Pilates, HIIT, Core, and more.",
    },
    {
      pict:
        "https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/categories/Mobile_Category_Mindfulness.jpg",
      name: "MINDFULNESS",
      desc: "Find meditations for relaxation, creativity, and restful sleep.",
    },
    {
      pict:
        "https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/categories/Mobile_Category_Skills.jpg",
      name: "SKILSS",
      desc:
        "Learn how to handstand or stretch into splits with guided instruction.",
    },
  ];

  let listInstructor = [
    {
      pict:
        "https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/instructors/Dylan_desktop.jpg",
      name: "Dylan Werner",
      desc: "Yoga Instructor",
    },
    {
      pict:
        "https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/instructors/Bri_desktop.jpg",
      name: "Briohny Smyth",
      desc: "Yoga Instructor",
    },
    {
      pict:
        "https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/instructors/Jacy_desktop.jpg",
      name: "Jacy Cunningham",
      desc: "Fitness Instructor",
    },
    {
      pict:
        "https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/instructors/Ashley_desktop.jpg",
      name: "Ashley Galvin",
      desc: "Yoga Instructor",
    },
    {
      pict:
        "https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/instructors/Jackie_desktop.jpg",
      name: "Jackie Stewart",
      desc: "Mindfulness Instructor",
    },
    {
      pict:
        "https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/instructors/Adrienne_desktop.jpg",
      name: "Adrienne Kimberley",
      desc: "Barre Instructor",
    },
    {
      pict:
        "https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/instructors/Callie_desktop.jpg",
      name: "Callie Gullickson",
      desc: "Fitness Instructor",
    },
    {
      pict:
        "https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/instructors/Carling_desktop.jpg",
      name: "Carling Harps",
      desc: "Yoga Instructor",
    },
  ];

  let listStories = [
    {
      pict:
        "https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/user_stories/images/Mobile_UserStory_Joe.jpg",
      user: "Joseph M.",
      title:
        "Having a practice put me in a place to be an example for my students.",
    },
    {
      pict:
        "https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/user_stories/images/Mobile_UserStory_Anna.jpg",
      user: "Anna V.",
      title:
        "Being surrounded by nature is crucial to my art and practice. They're woven together.",
    },
    {
      pict:
        "https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/user_stories/images/Mobile_UserStory_Penny.jpg",
      user: "Penny W.",
      title:
        "Yoga became a medicine for me. On Alo Moves, I found a support system.",
    },
  ];

  onMount(async () => {
    // document.getElementById("mainvideo").play();
  });
</script>

<!-- Navbar -->
<NavbarGuest />

<!-- Main Video -->
<div style="margin-top:73px; position: relative">
  <div class="main-hero-text align-middle text-center text-white">
    <h1 class="text-main">GO AFTER YOUR GOALS</h1>
    <h4 class="mt-1 mb-4 text-normal text-second">
      Need some extra motivation? Enjoy 50% off your first year of unlimited
      yoga, fitness, and meditation.
    </h4>
    <div class="mt-3 mb-4">
      <a href="#!" class="btn btn-light btn-lg text-arq btn-savenow">SAVE NOW</a
      >
    </div>
    <div class="mt-4">
      <a href="#!" class="text-white"><u>Send a Gift Card</u></a>
    </div>
  </div>
  <!-- svelte-ignore a11y-media-has-caption -->
  <video
    src="https://alomoves.s3.amazonaws.com/manual_uploads/shared/promotions/hero_black_friday_2020.webm"
    autoplay
    playsinline
    loop
    muted
    preload="auto"
    class="main-hero-video"
  />
</div>

<div class="container text-center py-4 my-4" style="max-width:900px">
  <h1 class="text-main">FIND WHAT MOVES YOU</h1>
  <h5 class="text-normal text-second text-secondary">
    Whether you’re a complete beginner or you want to step up your routine, get
    the full studio experience at home with thousands of classes for body, mind,
    and spirit.
  </h5>
</div>

<!-- List class -->
<div class="container my-4 py-4">
  <div class="row flex-row flex-nowrap">
    {#each listClass as { pict, name, desc }}
      <div class="col">
        <img src={pict} alt={name} width="100%" />
        <h5 class="mt-1 text-arq">
          {name}
          <span class="text-muted" style="margin-left:15px;font-size:30px"
            >&rsaquo;</span
          >
        </h5>
        <div class="text-muted text-prox" style="font-size:18px">{desc}</div>
      </div>
    {/each}
  </div>
</div>

<div style="margin-top:50px">
  <div class="fitimage">
    <div class="row">
      <div class="col-md" />
      <div class="col-md">
        <img
          src="https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/bleed_images/Mobile_Banner1.jpg"
          alt="Woman."
          width="100%"
        />
      </div>
    </div>
  </div>

  <div class="container space-top">
    <div class="row text-sm-start text-center">
      <div class="col-md px-4">
        <h1 class="text-main">FIT FOR YOUR LIFESTYLE</h1>
        <h5 class="text-normal text-second text-secondary mb-4">
          Wake up with a sunrise meditation, sweat it out with lunchtime HIIT,
          or unwind with an evening flow. You’ll find movement for every mood
          with classes sorted by time, style, and skill level.
        </h5>
        <div class="mt-4 pt-4">
          <a href="#!" class="btn btn-outline-dark btn-lg px-4"
            >EXPLORE CLASSES</a
          >
        </div>
      </div>
      <div class="col-md" />
    </div>
  </div>
</div>

<div class="container text-center" style="margin-top:280px;max-width:900px">
  <h1 class="text-main">MEET OUR INSTRUCTORS</h1>
  <h5 class="text-normal text-second text-secondary mb-4">
    Challenge your strength. Stretch your body. Breathe easy. Our team of
    world-class instructors will empower you to grow and achieve all of your
    fitness and wellness goals.
  </h5>
  <div class="mt-4 pt-4">
    <a href="#!" class="btn btn-outline-dark px-4 btn-lg">VIEW INSTRUCTORS</a>
  </div>
</div>

<!-- List instructor -->
<div class="container-fluid space-top" style="overflow:hidden">
  <div class="row flex-row flex-nowrap">
    {#each listInstructor as { pict, name, desc }}
      <div class="col-3" style="max-width:250px">
        <img src={pict} alt={name} width="100%" />
        <h6 class="text-arq text-uppercase mt-3 text-body">
          {name}
        </h6>
        <div class="text-prox text-muted">{desc}</div>
      </div>
    {/each}
  </div>
</div>

<div class="space-top">
  <div class="row text-sm-start text-center">
    <div class="col-md">
      <img
        src="https://alomoves.s3.amazonaws.com/manual_uploads/shared/home/bleed_images/Desktop_Banner2.jpg"
        alt="Woman."
        width="100%,,,55vw"
      />
    </div>
    <div class="col-md px-4">
      <div style="max-width:650px">
        <h1 class="text-main">FOR EVERY SPACE, AT ANY PACE</h1>
        <h5 class="text-normal text-second text-secondary mb-4">
          From the comfort of your living room to a hotel room across the globe,
          we put the best classes at your fingertips. No WiFi? Download videos
          offline for a practice that moves with you
        </h5>
        <div class="mt-4 pt-4">
          <a href="#!" class="btn btn-outline-dark btn-lg px-4"
            >EXPLORE CLASSES</a
          >
        </div>
      </div>
    </div>
  </div>
</div>

<div class="container text-center space-top" style="max-width:900px">
  <h1 class="text-main">STORIES FROM OUR COMMUNITY</h1>
  <h5 class="text-normal text-second text-secondary mb-4">
    From incorporating mindfulness in the classroom to having virtual yoga
    practice with friends around the world, tune in to see how our community
    uses Alo Moves.
  </h5>
</div>

<!-- List stories -->
<div class="container my-4 py-4">
  <div class="row">
    {#each listStories as { pict, user, title }}
      <div class="col">
        <img src={pict} alt={user} width="100%" />
        <div class="text-white p-4" style="margin-top:-155px">
          <h4 class="mt-2 text-normal text-prox">
            "{title}"
          </h4>
          <div class="text-arq text-uppercase">{user}</div>
        </div>
      </div>
    {/each}
  </div>
</div>

<div class="bg-dark">
  <div class="container space-top pb-4 text-light">
    <div class="row py-4">
      <div class="col-md">
        <h1 class="text-main">YOUR ALL-ACCESS PASS</h1>
        <h5 class="text-normal">
          This sale is too good to miss. Unlock unlimited classes with 50% off
          your first year.
        </h5>
      </div>
      <div class="col-md text-center align-middle">
        <a href="#!" class="btn btn btn-light btn-lg mr-4">SAVE NOW</a>
        <a href="#!" class="btn btn btn-outline-light btn-lg">EXPLORE</a>
      </div>
    </div>
  </div>
</div>

<Footer />

<style>
  .main-hero-video {
    width: 100%;
    height: 100%;
    display: block;
  }

  .main-hero-text {
    position: absolute;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.4);
    flex-direction: column;
    -webkit-box-pack: center;
    justify-content: center;
    display: flex;
    padding-top: 0px;
    z-index: 700;
  }

  .fitimage {
    position: absolute;
    width: 100%;
    margin-top: -100px;
  }

  .text-normal {
    font-weight: normal !important;
  }

  .space-top {
    margin-top: 160px;
  }

  .text-arq {
    font-family: "Arquitecta", Helvetica, Arial, sans-serif;
  }

  .text-prox {
    font-family: "Proxima-Nova", Helvetica, Arial, sans-serif;
  }

  .text-main {
    font-family: "Arquitecta", Helvetica, Arial, sans-serif;
    font-weight: 700;
    line-height: 105%;
    letter-spacing: 0.08em;
  }

  .text-second {
    font-family: "Proxima-Nova", Helvetica, Arial, sans-serif;
    letter-spacing: normal;
    line-height: 170%;
    font-weight: 300;
    text-transform: none;
  }

  .btn-savenow {
    min-width: 160px;
  }
  .btn-savenow:hover {
    background-color: rgb(36, 36, 36);
    border-color: rgb(36, 36, 36);
    color: rgb(255, 255, 255);
  }
</style>
