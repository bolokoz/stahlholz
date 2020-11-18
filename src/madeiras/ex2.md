---
meta:
  - name: description
    content: Rendering Local JSON Data 
  - name: keywords
    content: vuepress vue component local data json
---
# Rendering Local JSON Data

Use import to grab local json data and render its contents.


<div v-for="i in items">
    <Questao questao="i.questao"/>
    <Respostas respostas="i.respostas"/>
</div>

<demo-component msg="pudim"></demo-component>
<OtherComponent :msg="pudim"/>

<script>
import data from './exercicios.json'
export default {
  data () {
      return {
          items: data.exercicios
      }
  }
}
</script>
