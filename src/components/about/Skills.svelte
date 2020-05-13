<script>
  import skills from "./partials/_skills.js";
  import SkillsList from "./partials/SkillsList.svelte";
</script>

<style>
  #aboutSkillsText {
    line-height: 1;
  }

  #aboutSkillsTitle {
    margin-bottom: 15px;
  }
</style>

<div id="" class="greyWrapper extraMargin25 flexContainer">
  <div class="flexContent">
    <div id="aboutSkills">
      <h2 id="aboutSkillsTitle">Skills &amp; roles</h2>
      <div id="aboutSkillsText">
        {#each skills as skill}
          <SkillsList {skill} />
        {/each}
      </div>
    </div>
  </div>
</div>
