<script>
  export let edu;
</script>

<style>
  .eduWrapper {
    width: 100%;
    border: solid 1px #f1f1f1;
    background-color: #f5f5f5;
    padding: 15px;
    margin-bottom: 25px;
  }

  .eduWrapper a,
  .eduWrapper p {
    font-size: 14px;
  }

  .eduInversed {
    background-color: #444;
    color: #f5f5f5;
  }
  .eduInversed a,
  .eduInversed h3 {
    color: #f5f5f5;
  }

  @media screen and (min-width: 900px) {
    .eduWrapper {
      width: calc(33% - 15px);
      margin-right: 15px;
      margin-bottom: 15px;
      padding: 15px;
    }
  }
</style>

<div class="eduWrapper {edu.formal ? 'eduInversed' : ''}">
  <h3 class="eduTitle">{edu.title}</h3>
  <div class="eduContent">
    <p>{edu.year} @ {edu.institution}</p>
    <a rel="noopener noreferrer" target="_blank" href={edu.link}>
      {edu.linkName}
    </a>
  </div>
</div>
