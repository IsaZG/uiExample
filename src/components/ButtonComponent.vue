<template>
  <component
    :is="tag === 'button' ? 'button' : tag === 'a' ? 'a' : 'input'"
    class="btn"
    :class="'btn-' + variant"
    :type="type"
    :href="href"
    :role="role"
  >
    <slot></slot>
  </component>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component({
  props: {
    tag: String,
    type: String,
    variant: String,
    href: String,
    role: String
  }
})
export default class ButtonComponent extends Vue {}
</script>
