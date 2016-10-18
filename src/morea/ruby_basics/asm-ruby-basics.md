---
title: "Basic Ruby Skills"
published: true
morea_id: asm-ruby-basics
morea_type: assessment
morea_sort_order: 1
morea_outcomes_assessed:
  - out-ruby-basics
---

Basic Ruby Skills:

- Running interactive ruby (ibr)
- Creating and running a ruby file
- Creating ruby variables
- Using ruby to display information to the shell
- Using ruby to get user input from the shell
- Perform simple arithmetic operations with integers and floats

<link rel="stylesheet" href="https://cdn.oesmith.co.uk/morris-0.4.3.min.css">
<script src="//cdnjs.cloudflare.com/ajax/libs/raphael/2.1.0/raphael-min.js"></script>
<script src="https://cdn.oesmith.co.uk/morris-0.4.3.min.js"></script>

<div class="well">
  <div id="asm-github-basics" style="height: 250px;"></div>
</div>

<script>
Morris.Bar({
  element: 'asm-github-basics',
  hideHover: false,
  data: [
        { y: 'Very satisfactory (%)', num: 0 },
        { y: 'Satisfactory (%)', num: 0 },
        { y: 'Unsatisfactory (%)', num: 0 },
        { y: 'Absent (%)', num: 0 },
        ],
  xkey: 'y',
  ykeys: ['num'],
  resize: true,
  labels: ['Students']
});
</script>
