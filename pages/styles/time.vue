<template>
<div>
  <h1>{{time}}</h1>
</div>
</template>

<script>
export default {
    data: ()=> ({
        time: ''
    }),
  methods: {
    startTime() {
      var today = new Date();
      var h = today.getHours();
      var m = today.getMinutes();
      var s = today.getSeconds();
      m = this.checkTime(m);
      s = this.checkTime(s);
      this.time = h + ":" + m + ":" + s;
      setTimeout(this.startTime, 500);

    },
    checkTime(i) {
        if (i < 10) {
            i = "0" + i
        };
        return i;
    }
    
  },

  mounted() {
    this.startTime();
  }
}
</script>

<style>
@font-face {
  font-family: "Product Sans";
  font-style: normal;
  font-weight: 700;
  src: local("Open Sans"), local("OpenSans"),
    url(https://fonts.gstatic.com/s/productsans/v5/HYvgU2fE2nRJvZ5JFAumwegdm0LZdjqr5-oayXSOefg.woff2)
      format("woff2");
}

* {
  text-transform: none !important;
  letter-spacing: 0.04em;
  font-family: Product Sans;
}
</style>