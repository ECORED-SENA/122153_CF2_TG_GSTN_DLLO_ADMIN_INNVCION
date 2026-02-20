<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    
    p.mb-5 El siguiente mapa integra los criterios y especificidades de los conocimientos expuestos en el presente componente formativo:
    .row.justify-content-center
      .col-lg-10.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis.svg", alt="A continuación, se presenta la síntesis del componente formativo: normatividad, formalización de empresa, documentos e informes contables, en este encontramos: Hechos contables: los cuales constan de la cuenta y ecuación contable. Proceso administrativo: este cuenta con archivos y conservación de documentos, además, presenta el ciclo administrativo (planeación, organización, dirección y control). Obligación tributarias: hace referencia a los tipos de impuestos. Informes contables y estados financieros: nos presenta el informe de propósito general, estados financieros intermedios, estados financieros separados y finalmente estados financieros consolidados. Información contable: nos presenta información de usuarios, el periodo contable, los libros contables y las características y documentos, dichos documentos se presentan, internos, externos y extra contables o títulos valores. Contabilidad: nos expone los tipos de contabilidad los cuales son tributaria, gerencial y financiera, además nos plantea dos tipos de usuarios, internos y externos. Empresa: su clasificación es por su naturaleza, actividad económica, capital, ingresos y sector, presentación de información financiera, finalidad y forma de asociación.")
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
