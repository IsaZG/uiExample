<template>
  <li :class="'breadcrumb-' + variant">
    <slot></slot>
  </li>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component({
  props: {
    variant: String
  }
})
export default class BreadcrumbComponent extends Vue {}
</script>
