<template>
  <div class="teaching container-fluid">
    <div class="row mt-3">
      <div class="col-12">
        <teach-card v-for="t in filteredTeaching"
         :title="t.title"
         :year="t.year"
         :desc="t.desc"
         :tags="t.tags"
         :loc="t.location"
         :lesson="t.lesson"
         type="teach"
        >
        </teach-card>
      </div>
    </div>
  </div>
</template>

<script>
import teachCard from './TeachCard';

export default {
  name: 'HelloWorld',
  components: { teachCard },
  props: ['filter'],
  computed: {
    filteredTeaching() {
      return this.teaching.filter(def =>
        def.title.toLowerCase().includes(this.filter.toLowerCase()) ||
        def.tags.toLowerCase().includes(this.filter.toLowerCase()) ||
        def.desc.toLowerCase().includes(this.filter.toLowerCase()) ||
        def.location.toLowerCase().includes(this.filter.toLowerCase())
      );
    },
  },
  data() {
    return {
      teaching: [
        {
          title: 'Sleep and Neuroimaging Laboratory',
          year: 2018,
          desc: 'Co-­organized and taught workshop on resting state connectivity analyses',
          tags: 'javascript, data science',
          location: 'University of California, Berkeley',
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
