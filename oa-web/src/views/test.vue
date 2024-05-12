<template>
  <div>
    <div>账号切换</div>
    <button @click="admin()" type="default" size="mini">admin</button>
    <button @click="zhangsan()" type="default" size="mini">张三</button>
    <button @click="lisi()" type="default" size="mini">李四</button>
    <div>当前token：{{ token }}</div>
  </div>
</template>

<script>
export default {
  name: "Test",

  data() {
    return {
      token: ''
    };
  },

  created(){
    this.token = window.localStorage.getItem('token')
  },

  methods: {
    admin() {
      window.localStorage.setItem('token', '');
      let token = 'eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDM3NjMwNDIx1FEqLU4t8kxRsjKCMPMSc1OBWsqzcpRqAb4pVZBAAAAA.-bW4hJ5UptFiCRsL6jVUa4XbgVwdsfVGfP8gJ-tOVbp7D3JOb8sylbBDLUhTZt6FJsYhlA5uYz8HSRck_pbaCA'
      window.localStorage.setItem('token', token);
      this.token = window.localStorage.getItem('token')
    },

    zhangsan() {
      window.localStorage.setItem('token', '');
      let token = 'eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDc0Mzc0MrE01FEqLU4t8kxRsjKHMPMSc1OBWqoyEvPSixPzlGoB3_ce3EUAAAA.2TVuQDaX_4rZ0_YKc1unEngGaZ3-HcoUIlDC-bYMkpWwOZa2BWRD9PblIRt1FqWeZzFqZ6pEA-jgQm58MpsYEA'
      window.localStorage.setItem('token', token);
      this.token = window.localStorage.getItem('token')
    },

    lisi() {
      window.localStorage.setItem('token', '');
      let token = 'eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDc0Mzc0MrUw11EqLU4t8kxRsjKBMPMSc1OBWnIyizOVagEBjHoLQQAAAA.6eCaG10EW7in6UjbGGmfJuoe9oqH9vYrnHtH9mEMo3uyK43p53eLsBJQGFvAgrNEyeAF3G6ihQ3q54C0BxRHoA'
      window.localStorage.setItem('token', token);
      this.token = window.localStorage.getItem('token')
    }
  }
}
</script>
