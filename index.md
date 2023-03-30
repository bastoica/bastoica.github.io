---
layout: about
permalink: /
profile:
  align: right
  image: profile.png
published: true
---

<!--
<hr class="news-style" style="width: 95%; ">
-->

I am a Systems PhD student in the Computer Science Department at the University of Chicago. 
I am fortunate to be advised by Prof. <a href="https://people.cs.uchicago.edu/~shanlu/" target="_blank">Shan Lu</a>, and mentored by Dr. <a href="https://www.microsoft.com/en-us/research/people/sumann/" target="_blank">Suman Nath</a> and Dr. <a href="https://www.microsoft.com/en-us/research/people/madanm/" target="_blank">Madan Musuvathi</a> from Microsoft Research. 
My doctoral studies are supported, in part, by an [Eckhardt Scholarship](https://physicalsciences.uchicago.edu/academics/financial-aid/eckhardt-scholars/).

My research focuses on improving the correctness and performance of large-scale distributed systems.
I build tools rooted in program analysis, code instrumentation, fault injection, and execution profiling to help developers better reason about their code and isolate bugs faster.

Before joining UChicago, I obtained my MSc degree from the Swiss Federal Institute of Technology in Lausanne (EPFL) and my BSc degree from the University of Bucharest.
In another lifetime, I had a grown-up job working as a Software Engineer for Microsoft and Bitdefender Labs.

<h4 class="news-style">Recent News</h4>
<hr class="news-style" style="width: 95%; ">


<table id="newsTable" style="border-collapse: collapse;">
  <tr>
    <td style="padding-bottom: 10px; text-align: left;"><i>August<br>2022</i></td>
    <td style="padding-bottom: 10px; padding-left: 20px; text-align: left;">Our paper on exposing memory order violations using delay injection was accepted at EuroSys'23. See you in Rome!</td>
  </tr>
  <tr>
    <td style="padding-bottom: 10px; text-align: left;"><i>March<br>2022</i></td>
    <td style="padding-bottom: 10px; padding-left: 20px; text-align: left;">This summer, I will join the Profiling group at Meta as a Research Intern mentored by Nathan Slingerland.</td>
  </tr>
  <tr>
    <td style="padding-bottom: 10px; text-align: left;"><i>February<br>2022</i></td>
    <td style="padding-bottom: 10px; padding-left: 20px; text-align: left;">I will serve on the Artifact Evaluation committees of ASPLOS'22, EuroSys'22 and OSDI'22. Please consider submitting your code.</td>
  </tr>
  <tr>
    <td style="padding-bottom: 10px; text-align: left;"><i>August<br>2021</i></td>
    <td style="padding-bottom: 10px; padding-left: 20px;  text-align: left;">I will serve on the Artifact Evaluation Committee of SOSP'21. Please consider registring your artifacts.</td>
  </tr>
  <tr>
    <td style="padding-bottom: 10px; text-align: left;"><i>January<br>2021</i></td>
    <td style="padding-bottom: 10px; padding-left: 20px;  text-align: left;">This winter, I will join Microsoft Research as a PhD Collaborator, mentored by Dr. Suman Nath and Dr. Madan Musuvathi. </td>
  </tr>
</table>


<script>
  function showMore() {
    var table = document.getElementById("newsTable");
    var rows = table.getElementsByTagName("tr");

    // Show the next n-3 rows
    for (var i = 3; i < rows.length; i++) {
      rows[i].style.display = "table-row";
    }

    // Hide the "Show more" button
    document.getElementById("showMoreBtn").style.display = "none";

    // Show the "Show less" button
    document.getElementById("showLessBtn").style.display = "inline-block";
  }

  function showLess() {
    var table = document.getElementById("newsTable");
    var rows = table.getElementsByTagName("tr");

    // Hide the last n-3 rows
    for (var i = 3; i < rows.length; i++) {
      rows[i].style.display = "none";
    }

    // Show the "Show more" button
    document.getElementById("showMoreBtn").style.display = "inline-block";

    // Hide the "Show less" button
    document.getElementById("showLessBtn").style.display = "none";
  }
</script>

<button id="showMoreBtn" onclick="showMore()">Show more...</button>
<button id="showLessBtn" onclick="showLess()" style="display: none;">Show less...</button>

<style>
  /* Hide rows 4 and beyond by default */
  #newsTable tr:nth-child(n+4) {
    display: none;
  }
</style>
