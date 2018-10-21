<template>
  <div class="skills">
    <span
      v-for="(skill, index) in skills"
      :key="index"
      :class="[`text-${kebab(skill.label)}`, {'font-medium': skill.weight == 1, 'font-semibold': skill.weight == 2}]"
      class="skill"
      v-text="skill.label"/>
  </div>
</template>

<script>
export default {
  props: {
    skills: {
      type: Array,
      default: () => {
        return []
      }
    }
  },

  methods: {
    kebab(string)
    {
      return string.replace(/([a-z])([A-Z])/g, "$1-$2")
                  .replace(/\s+/g, '-')
                  .toLowerCase();
    }
  }
}
</script>
