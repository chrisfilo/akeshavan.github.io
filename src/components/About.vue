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
                  <h4 class="title">Arielle Tambini, Ph.D.<br>
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
          
          <div class="content">
            <p class=""> <strong style="color:#e34a33">I'm starting a lab at UC Irvine!</strong><br> Research in the lab will focus on understanding systems-level mechanisms
            and brain states that support long-term memory retention in humans, combining correlational approaches (fMRI, behavior)
            with causal manipulations (TMS, targeted memory reactivation).</p>
            <p class=""><b>Interested in joining the lab?</b> 
            <br>I'm currently recruiting:
            <br>- a full-time Research Assistant/Lab Manager,
            <br>- Ph.D. students,
            <br>- Undergraduate Research Assistants.</p>
            <p>Prospective Ph.D. students should apply through the 
            <a href=https://inp.uci.edu/>UCI Interdepartmental Neuroscience Program.</a>
            If you are interested in joining, please get in touch with me at atambini_at_uci_dot_edu</p>

          </div>
        </div>
      </div>


      </div>
      <div class="col-lg-6 col-md-12">
        <div class="card">
          <div class="header">
            <h5 class="title">Prior Education & Training</h5>
            
          </div>
          <div class="content">
            <p>Postdoctoral Research Fellow<br>University of California, Berkeley<br>(2013-2019)</p>
          </div>
          <div class="content">
            <p>Ph.D. in Neural Science<br> New York University<br>(2007-2013)</p>
          </div>
          <div class="content">
            <p>B.S. in Brain & Cognitive Sciences (minor in Biomedical Engineering)<br>
            Massachusetts Institute of Technology<br>(2003-2007)</p>
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
