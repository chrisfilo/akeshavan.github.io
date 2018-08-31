<template>
  <div class="hello container-fluid">
    <div class="row mt-3">
      <div class="col-12">
        <pub-card v-for="p in filteredPublications"
         :title="p.title"
         :authors="p.authors"
         :link="p.link"
         :year="p.year"
         :journal="p.journal"
         :tags="p.tags">
        </pub-card>
      </div>
    </div>
  </div>
</template>

<script>
import pubCard from './PubCard';

export default {
  name: 'Publications',
  components: {pubCard},
  props: ['filter'],
  computed: {
    filteredPublications() {
      return this.publications.filter(def =>
        def.title.toLowerCase().includes(this.filter.toLowerCase()) ||
        def.authors.toLowerCase().includes(this.filter.toLowerCase()) ||
        def.tags.toLowerCase().includes(this.filter.toLowerCase())
      );
    },
  },
  data() {
    return {
      publications: [
        {
          title: 'Hippocampal-targeted Theta-burst Stimulation Enhances Associative Memory Formation.',
          authors: 'A Tambini, DE Nee, M D\'Esposito',
          link: 'http://doai.io/10.1162/jocn_a_01300',
          year: '2018',
          journal: 'Journal of cognitive neuroscience, 1-21',
        },
        {
          title: 'Spontaneous cognitive processes and the behavioral validation of time-varying brain connectivity.',
          authors: 'A Kucyi, A Tambini, S Sadaghiani, S Keilholz, JR Cohen',
          link: 'http://doai.io/10.1162/netn_a_00037',
          year: '2018',
          journal: 'Network Neuroscience, 1-57',
        },
        {
          title: 'Brief targeted memory reactivation during the awake state enhances memory stability and benefits the weakest memories.',
          authors: 'A Tambini, A Berners-Lee, L Davachi',
          link: 'http://doai.io/10.1038/s41598-017-15608-x',
          year: '2017',
          journal: 'Scientific Reports 7 (1), 15325',
        },
        {
          title: 'Persistence of amygdala–hippocampal connectivity and multi-voxel correlation structures during awake rest after fear learning predicts long-term expression of fear.',
          authors: 'EJ Hermans, JW Kanen, A Tambini, G Fernández, L Davachi, EA Phelps',
          link: 'http://doai.io/10.1093/cercor/bhw145',
          year: '2017',
          journal: 'Cerebral Cortex 27 (5), 3028-3041',
        },
        {
          title: 'Emotional brain states carry over and enhance future memory formation.',
          authors: 'A Tambini, U Rimmele, EA Phelps, L Davachi',
          link: 'http://doai.io/10.1038/nn.4468',
          year: '2017',
          journal: 'Nature neuroscience 20 (2), 271',
        },
        {
          title: 'Sleep, Sleep Alterations, Stress—Combined Effects on Memory?',
          authors: 'U Rimmele, A Tambini',
          link: 'http://doai.io/10.5665/sleep.5214',
          year: '2015',
          journal: 'Sleep 38 (12), 1835-1836',
        },
        {
          title: 'Persistence of hippocampal multivoxel patterns into postencoding rest is related to memory.',
          authors: 'A Tambini, L Davachi',
          link: 'http://doai.io/10.1073/pnas.1308499110',
          year: '2013',
          journal: 'Proceedings of the National Academy of Sciences 110 (48), 19591-19596',
        },
        {
          title: 'Enhanced brain correlations during rest are related to memory for recent experiences.',
          authors: 'A Tambini, N Ketz, L Davachi',
          link: 'http://doai.io/10.1016/j.neuron.2010.01.001',
          year: '2010',
          journal: 'Neuron 65 (2), 280-290',
        },
        {
          title: 'Sensory contributions to impaired emotion processing in schizophrenia.',
          authors: 'PD Butler, IY Abeles, NG Weiskopf, A Tambini, M Jalbrzikowski, ME Legatt, V Zemon, J Loughead, RC Gur, DC Javitt',
          link: 'http://doai.io/10.1093/schbul/sbp109',
          year: '2009',
          journal: 'Schizophrenia bulletin 35 (6), 1095-1107',
        },
        {
          title: 'The asymmetry of the fusiform face area is a stable individual characteristic that underlies the left-visual-field superiority for faces.',
          authors: 'G Yovel, A Tambini, T Brandman',
          link: 'http://doai.io/10.1016/j.neuropsychologia.2008.06.017',
          year: '2008',
          journal: 'Neuropsychologia 46 (13), 3061-3068',
        },
        {
          title: 'What\'s in a face? Effects of stimulus duration and inversion on face processing in schizophrenia.',
          authors: 'PD Butler, A Tambini, G Yovel, M Jalbrzikowski, R Ziwich, G Silipo, N Kanwisher, DC Javitt',
          link: 'http://doai.io/10.1016/j.schres.2008.03.007',
          year: '2008',
          journal: 'Schizophrenia research 103 (1-3), 283-292',
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
