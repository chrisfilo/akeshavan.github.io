<template>
  <div class="awards container-fluid">
    <div class="row mt-3">
      <div class="col-12">
        <teach-card v-for="t in filteredTeaching"
         :title="t.title"
         :year="t.year"
         :desc="t.desc"
         :tags="t.tags"
         :loc="t.location"
         :lesson="t.lesson"
         type="awards"
        >
        </teach-card>
      </div>
    </div>
  </div>
</template>

<script>
import teachCard from './TeachCard';

export default {
  name: 'Awards',
  components: { teachCard },
  props: ['filter'],
  computed: {
    filteredTeaching() {
      return this.teaching.filter(def =>
        def.title.toLowerCase().includes(this.filter.toLowerCase()) ||
        def.tags.toLowerCase().includes(this.filter.toLowerCase()) ||
        def.desc.toLowerCase().includes(this.filter.toLowerCase())
      );
    },
  },
  data() {
    return {
      teaching: [
        {
          title: 'Ruth L. Kirschstein NRSA Postdoctoral Fellowship',
          year: '2015-2018',
          desc: 'F32 MH106280',
          tags: null,
          location: null,
          lesson: null,
        },
        {
          title: 'Ruth L. Kirschstein NRSA Predoctoral Fellowship',
          year: '2010-2013',
          desc: 'F31 MH092055',
          tags: null,
          location: null,
          lesson: null,
        },
        {
          title: 'Marine Biological Laboratory Neuroinformatics Summer Course scholarship',
          year: 2011,
          desc: null,
          tags: null,
          location: null,
          lesson: null,
        },
        {
          title: 'NYU Dean’s Student Travel Grant',
          year: '2009-2011',
          desc: 'received max. of 3 times',
          tags: null,
          location: null,
          lesson: null,
        },
        {
          title: 'Hans-Lukas Teuber Award for Outstanding Academics',
          year: 2007,
          desc: 'Department of Brain and Cognitive Sciences, MIT',
          tags: null,
          location: null,
          lesson: null,
        },
        {
          title: 'Summer Scholars Program in Biomedical Optics',
          year: 2005,
          desc: 'Harvard/MIT Division of Health Sciences and Technology',
          tags: null,
          location: null,
          lesson: null,
        },
        {
          title: 'Davidson Fellowship',
          year: 2003,
          desc: '$10,000 award for original research',
          tags: null,
          location: null,
          lesson: null,
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
