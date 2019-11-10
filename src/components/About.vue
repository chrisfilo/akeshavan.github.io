<template>
  <div class="about container">
    <div class="row mt-3">
      <div class="col-lg-6 col-md-12">
        <div class="card card-user">
            <div class="image">
                <img src="../assets/img/new_york.jpg" alt="...">
            </div>
            <div class="content">
                <div class="author">
                  <img class="avatar border-white" src="../assets/img/faces/arielle_portrait.jpg" alt="...">
                  <h4 class="title">Arielle Tambini, PhD<br>
                  <a href="https://scholar.google.com/citations?user=ZRiWbw0AAAAJ&hl=en"><small>Google Scholar</small></a>
                  </h4>
                </div>
                <p class="description text-center">
                    Assistant Professor, <a href="https://neurobiology.uci.edu/">Department of Neurobiology and Behavior</a>
                    <br>
                    University of California, Irvine
                    <br>
                    (starting in January 2020!)
                    
                </p>
            </div>
            <hr>
            <div class="text-center">
                <div class="row">
                    <div class="col-md-12">
                        <p class="description pl-2 pr-2">
                          <span class="text-info">Interests:</span>
                          Cognitive Neuroscience,
                          Memory Consolidation,
                          Rest,
                          Hippocampus,
                          fMRI,
                          TMS,
                          Bagels
                        </p>
                    </div>
                </div>
            </div>
        </div>

      </div>
      <div class="col-lg-6 col-md-12">
        <div class="card">
          <div class="header">
            <h4 class="title">Education</h4>
            <p class="category">
              Where I've Learned
            </p>
          </div>
          <div class="content">
          <div class="typo-line mt-3">
            <h6><p class="category">Postdoc<br>2013-2019</p>Cognitive Neuroscience</h6>
            <p class="text-muted">University of California, Berkeley</p>
            <p class="">Advisor: Mark D'Esposito</p>
          </div>

            <div class="typo-line mt-3">
              <h6 class="mb-2">
                <p class="category">
                  PhD
                  <br>2007-2013
                </p>
                Neural Sciences
              </h6>
              <p class="text-muted">New York University</p>

                <p>Advisor: Lila Davachi</p>


            </div>
            <div class="typo-line mt-3">
              <h6><p class="category">BS<br>2007-2011</p>Brain and Cognitive Sciences</h6>
              <p class="text-muted">Massachusetts Institute of Technology</p>
              <p class="">minor in Biomedical Engineering</p>
            </div>
          </div>
        </div>
      </div>
    </div>






  </div>
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
      msg: 'I\'m Arielle',
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

blockquote {
    font-style: italic;
    border-left: 5px solid #eee;
    padding: 10px 20px;
    margin: 0 0 20px;
}
</style>
