<template>
  <div>
    <h1 id="logo">
      <svg
        id="LogoMedin"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 700 265"
        :style="{fill: color}"
      >
        <switch>
          <g>
            <path
              d="M208 253h88.1v-25.2h-61.5V180h59.8v-25.3h-59.8v-33.3h61.5V96.1H208zM87.1 201.3L33.8 80.5 0 253h27.6l15.7-88.5 43.4 98.1 44.6-97.9 14.1 88.3h27.4L142.4 80.4zM428.5 174.6c0 16.1-5.6 29.3-16.5 39.3-5.4 4.8-11.4 8.4-18 10.7-6.7 2.1-15.2 3.2-25.4 3.2h-8.7V121.4h8.7c19.2 0 33.9 4.6 43.6 13.5 10.8 10.1 16.3 23.4 16.3 39.7m2.6-58.3c-8-7.3-17-12.5-26.8-15.6-9.1-3.1-21.6-4.7-37.1-4.7h-34v157h33.6c15.7 0 28-1.5 36.6-4.4 9.3-2.9 18.2-8.1 26.7-15.6 16.8-14.9 25.3-34.6 25.3-58.6 0-23.8-8.2-43.4-24.3-58.1"
            />
            <g class="lighten">
              <path
                class="st0"
                d="M561.4 253h26.7V148.2L700 265V96.1h-26.7v104L561.4 83zM491.7 90.9h26.7v161.6h-26.7z"
              />
              <path
                class="st0"
                d="M505.1 0c-15.4 0-27.9 12.5-27.9 27.9 0 15.4 12.5 27.9 27.9 27.9 15.4 0 27.9-12.5 27.9-27.9C533 12.5 520.5 0 505.1 0"
              />
            </g>
          </g>
        </switch>
      </svg>
    </h1>
    <h2>Biel / Bienne</h2>
  </div>
</template>

<script>
export default {
  name: "Head",
  props: ["color"]
};
</script>

<style lang="stylus" scoped>
h1 {
  margin-bottom: 0;
}

h2 {
  margin-bottom: 3rem;
}

#LogoMedin {
  height: 4rem;
  fill: blue;
  transition: fill 2s ease-in-out;
}
</style>

