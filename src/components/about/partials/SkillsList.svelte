<script>
  export let skill;
</script>

<style>
.role, .skill {
    display: inline-block;
    background-color: var(--light-grey-color);
    border: solid 1px #fff;
    margin: 5px 15px 0 0;
}
.role {
    background-color: var(--darker-grey-color);
    color: #fff;
}
.skillName {
    padding: 5px 15px;
    font-size: 14px;
}
.proficiency {
    height: 2px;
    background-color: var(--dark-grey-color);
}
</style>

<div title={"Proficiency: " + skill.proficiency + "%"} class={skill.isSkill ? 'skill' : 'role'}>
  <div class="skillName">{skill.name}</div>
  <div style={"width:" + skill.proficiency + "%"} class="proficiency">&nbsp;</div>
</div>
