<script>
  import { Jobs, Edus } from "./partials/_career.js";
  import CareerList from "./partials/CareerList.svelte";
  import EduList from "./partials/EduList.svelte";
</script>

<style>
  #aboutJobsTitle {
    margin-bottom: 15px;
  }

  #aboutEduText {
    display: block;
    margin: 25px 0;
  }
  @media screen and (min-width: 900px) {
    #aboutJobsTitle {
      margin-bottom: 25px;
    }

    #aboutEduText {
      display: flex;
      flex-wrap: wrap;
    }
  }
</style>

<div id="" class="flexContainer">
  <div class="flexContent">
    <div id="aboutJobs" class="extraBottomMargin25">
      <h2 id="aboutJobsTitle">Career</h2>
      <div id="aboutJobsText">
        {#each Jobs as job}
          <CareerList {job} />
        {/each}
      </div>
    </div>

    <div class="dottedFlex">
      <hr class="dottedLine extraBottomMargin25" />
    </div>

    <div id="aboutEdu">
      <h2 id="aboutEduTitle">
        Education
        <span class="small grey">*outside of learning every day</span>
      </h2>
      <div id="aboutEduText">
        {#each Edus as edu}
          <EduList {edu} />
        {/each}
      </div>
    </div>
  </div>
</div>
