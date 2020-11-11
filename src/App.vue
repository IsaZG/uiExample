<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <ui-compone />
    <ui-comptwo />
    <h3>Alerts</h3>
    <AlertComponent variant="warning">Hello</AlertComponent>
    <AlertComponent variant="info">Hello</AlertComponent>
    <AlertComponent variant="light">Hello</AlertComponent>
    <AlertComponent variant="dark">Hello</AlertComponent>
    <AlertComponent variant="success">
      Hello
      <a href="www.google.com" class="alert-link">with link</a>
    </AlertComponent>
    <AlertComponent variant="danger" dismissing>Hello</AlertComponent>
    <AlertComponent variant="success">
      <h4 class="alert-heading">This is the title</h4>
      <p>This is the content</p>
      <hr />
      <p class="mb-0">Here we have more content</p>
    </AlertComponent>
    <h3>Badges</h3>
    <BadgeComponent type="regular" variant="secondary"
      >Simple Badge</BadgeComponent
    >
    <BadgeComponent type="button" variant="primary"
      >Notification 5</BadgeComponent
    >
    <BadgeComponent type="link" href="#" variant="success"
      >Link Badge</BadgeComponent
    >
    <BadgeComponent variant="pill badge-dark">Simple Badge</BadgeComponent>
    <BadgeComponent variant="pill badge-warning">Simple Badge</BadgeComponent>
    <h3>Breadcrumbs</h3>
    <nav aria-label="breadcrumb">
      <ol class="breadcrumb">
        <BreadcrumbComponent variant="item">
          <a href="#">Home</a>
        </BreadcrumbComponent>
        <BreadcrumbComponent variant="item">
          <a href="#">Next</a>
        </BreadcrumbComponent>
        <BreadcrumbComponent variant="item active" aria-current="page"
          >Next</BreadcrumbComponent
        >
      </ol>
    </nav>
    <h3>Buttons</h3>
    <ButtonComponent tag="button" variant="primary" type="button"
      >Primary</ButtonComponent
    >
    <br />
    <ButtonComponent tag="button" variant="secondary" type="button"
      >Secondary</ButtonComponent
    >
    <br />
    <ButtonComponent tag="button" variant="success" type="button"
      >Success</ButtonComponent
    >
    <br />
    <ButtonComponent tag="a" href="#" variant="primary" role="button"
      >Hi there!</ButtonComponent
    >
    <br />
    <ButtonComponent tag="button" variant="primary" type="submit"
      >Hey you!</ButtonComponent
    >
    <br />
    <ButtonComponent tag="a" variant="primary" type="submit" value="Input"
      >Testing!</ButtonComponent
    >
    <br />
    <ButtonComponent tag="button" variant="outline-primary"
      >Test!</ButtonComponent
    >
    <br />
    <ButtonComponent tag="button" variant="outline-danger"
      >Danger</ButtonComponent
    >
    <br />
    <ButtonComponent tag="button" variant="secondary btn-lg" type="button"
      >Large Button</ButtonComponent
    >
    <br />
    <ButtonComponent tag="button" variant="primary btn-sm" type="button"
      >Small Button</ButtonComponent
    >
    <br />
    <ButtonComponent
      tag="button"
      variant="primary btn-lg btn-block"
      type="button"
      >Block Button</ButtonComponent
    >
    <br />
    <ButtonComponent
      tag="a"
      variant="primary btn-lg active"
      role="button"
      aria-pressed="true"
      href="#"
      >Primary link</ButtonComponent
    >
    <br />
    <ButtonComponent
      tag="button"
      variant="lg btn-primary"
      type="button"
      disabled
      >Disabled</ButtonComponent
    >
    <br />
    <ButtonComponent
      tag="button"
      variant="primary"
      data-toggle="button"
      aria-pressed="false"
      >Single Toogle</ButtonComponent
    >
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import HelloWorld from "./components/HelloWorld.vue";
import AlertComponent from "./components/AlertComponent.vue";
import BadgeComponent from "./components/BadgeComponent.vue";
import BreadcrumbComponent from "./components/BreadcrumbComponent.vue";
import ButtonComponent from "./components/ButtonComponent.vue";

@Component({
  components: {
    HelloWorld,
    AlertComponent,
    BadgeComponent,
    BreadcrumbComponent,
    ButtonComponent
  }
})
export default class App extends Vue {}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
