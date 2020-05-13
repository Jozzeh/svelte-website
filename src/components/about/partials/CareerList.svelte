<script>
  export let job;
</script>

<style>
  .jobsWrapper {
    padding: 15px;
    border: solid 1px #f1f1f1;
    margin-bottom: 25px;
  }

  .jobsHeader {
    border-bottom: solid 2px #ccc;
    margin-bottom: 10px;
  }
  .jobsContent,
  .jobsHeader {
    padding-bottom: 10px;
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    align-items: flex-start;
  }

  .jobsCompany,
  .jobsYear {
    font-size: 14px;
    color: #666;
  }
  .jobsCompany,
  .jobsResponsibility,
  .jobsTech,
  .jobsTitle,
  .jobsYear {
    width: 100%;
    padding-bottom: 5px;
  }

  .jobsResponsibility,
  .jobsTech {
    margin: 10px 0;
    width: 100%;
  }

  .jobsResponsibilityTitle,
  .jobsTechTitle {
    padding-bottom: 10px;
    margin-bottom: 15px;
    border-bottom: solid 1px #ccc;
  }

  .jobsTechText {
    display: flex;
    flex-wrap: wrap;
    font-size: 16px;
  }

  .techstack {
    padding: 5px;
    margin: 5px;
    border: solid 1px #f1f1f1;
    background-color: #f5f5f5;
  }

  .jobsResponsibilityText p {
    margin-top: 0;
    font-size: 16px;
  }

  @media screen and (min-width: 900px) {
    .jobsContent,
    .jobsHeader {
      padding: 0 10px 10px 10px;
      width: calc(100% - 20px);
    }

    .jobsHeader {
      flex-wrap: nowrap;
      align-items: flex-end;
    }

    .jobsCompany,
    .jobsTitle,
    .jobsYear {
      padding-bottom: 0;
    }
    .jobsCompany,
    .jobsYear {
      width: 120px;
    }

    .jobsTitle {
      width: auto;
      flex: 1;
      text-align: center;
    }

    .jobsCompany {
      text-align: right;
    }

    .jobsResponsibility {
      margin-right: 5px;
    }

    .jobsResponsibility,
    .jobsTech {
      width: calc(50% - 5px);
      margin-top: 15px;
      margin-bottom: 0;
    }
  }
</style>

<div class="jobsWrapper">
  <div class="jobsHeader">
    <div class="jobsYear">{job.year}</div>
    <h3 class="jobsTitle">{job.title}</h3>
    <div class="jobsCompany">{job.company}</div>
  </div>
  <div class="jobsContent">
    <div class="jobsResponsibility">
      <div class="jobsResponsibilityTitle">Responsibilities</div>
      <div class="jobsResponsibilityText">
        <p>{job.responsibilities}</p>
      </div>
    </div>
    <div class="jobsTech">
      <div class="jobsTechTitle">Tech - Stack</div>
      <div class="jobsTechText">
        {#each job.tech as tech}
          <div class="techstack">{tech}</div>
        {/each}
      </div>
    </div>
  </div>
</div>
