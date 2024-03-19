<script setup>
import Document from '@/components/Document.vue'

const documentUrl = 'http://writing.engr.psu.edu/workbooks/formal_report_template.doc'
</script>

<template>
  <Document :url="documentUrl" :height="`900px`" />
</template>
