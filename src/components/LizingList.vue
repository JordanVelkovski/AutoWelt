<template>
  <div class="row">
    <h2 class="col-10 mx-auto fw-bold">Чекори за купување возило на лизинг:</h2>
    <ul class="col-10 mx-auto mt-2" v-for="id in objectList">
      <li class="list-unstyled mb-0">{{id.id}}.{{id.title}}</li>
      <p class="mb-0">{{id.innerBody}}</p>
    </ul>
  </div>
</template>

<script>
export default {
name: "LizingList",
data(){
  return {
      objectList: [
        {
          id : 1,
          title: 'ИЗБЕРЕТЕ ГО ВОЗИЛОТО',
          innerBody : 'Најпрво го избирате возилото кое сакате да го купите и добивате понуда за истото.\n' +
              '        Според изборот и понудата се подготвуваат потребните документи.'
        },
        {
          id : 2,
          title: 'НАШИТЕ ВРАБОТЕНИ ЌЕ ВИ ГИ ПОБАРААТ ПОТРЕБНИТЕ ПОДАТОЦИ',
          innerBody : 'Ги оставате сите потребни податоци на нашите вработени за да ја подготват целокупната\n' +
              '        документација која е потребна за аплицирање за лизингот.'
        },
        {
          id : 3,
          title: 'ПРЕДОДОБРУВАЊЕ',
          innerBody : 'Според податоците се преминува на фазата за пред-одобрување која ги елиминира или намалува можностите да бидете одбиени.\n' +
              '        Затоа е потребно податоците кои ќе ги оставите да бидат точни и прецизни.\n' +
              '        Лизинг копманијата ја разгледаува вашата апликација и дололку се е во ред ќе Ви го одобрат лизингот и ќе ве известат за тоа.\n' +
              '        Дополнително ќе ви ги кажат понатамошните чекори.'
        },
        {
          id : 4,
          title: 'КАПАР',
          innerBody : 'Доколку помине постапката на пред-одобрување потребно е да оставите капар за избраното возило за да ви\n' +
              '        биде резервирано се до конечно одобрувањето од банката.'
        },
        {
          id : 5,
          title: 'ПРЕЗЕМАЊЕ НА ВОЗИЛОТО',
          innerBody : 'Откако ќе се завршите целата процедура и лизингот ќе биде одобрен се договара датумот за превземање на возилото.'
        }

      ]
    }
  }
}
</script>

<style scoped>

</style>