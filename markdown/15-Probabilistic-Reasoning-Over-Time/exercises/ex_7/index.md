---
layout: exercise
title: Exercise 15.7
permalink: /dbn-exercises/ex_7/
breadcrumb: 15-Probabilistic-Reasoning-Over-Time
breadcrumb2: ex_7
breadcrumb3: 15probabilisticReasoningOverTime
---

{% include mathjax_support %}


<div class="card">
    <div class="card-header p-2">
        <a href='#' class="p-2">Exercise 7
        </a>

        <a class="solve_question" id="solve_question" href="#">
        <button type="button" class="btn btn-dark float-right" title="Solve this Exercise" href="#" id="buttonsolve">
        <i id="ex15.7" class="fas fa-pen" style="color:white"></i>
        </button>
        </a>

        <a class="edit_question" id="editt_question" href="#">
        <button type="button" class="btn btn-dark float-right" title="Edit this Question" style="margin-left:10px; margin-right:10px;" onclick="edit('ex15.7');" href="#" id="buttonsolve">
        <i id="ex15.7" class="far fa-edit" style="color:white"></i>
        </button>
        </a>

    </div>
    <div class="card-body">
        <p class="card-text">{% include_relative question.md %}</p>
    </div>
</div>

<br>
<div class="card">
    <div class="card-header p-2">
        <a href="#" class="p-2">Answers</a>


        <button type="button" class="btn btn-dark float-right" title="View Answers" id="viewanswers" onclick="myFunction()">
        <i id="view_answers1" class="fas fa-bars" style="color:white"></i>
        </button>

</div>
<div class="card-body" id="hideandviewanswers">
{% for item in site.data.answers.15probabilisticReasoningOverTime.ex_7.solutions %}
<div class="card">
   <div class="card-header p-2">
      <a href="#" class="p-2">Author: {{item.name}}</a>
      <a class="upvote_answer" id="upvote_answer" href="#">
      <button type="button" class="btn btn-dark float-right" title="Upvote answer" style="margin-left:10px; margin-right:10px;" href="#" id="upvoteanswer">
      <i class="far fa-thumbs-up" style="color:white"></i>
      </button>
      </a>
      </div>
<div class="card-body">
<p class="card-text">
{% for entry2 in item.answers %}
{{entry2.answer}}
{% endfor %}
</p>
<div class="card">
   <div class="card-header p-2">
      <a href="#" class="p-2">Comments</a>

      <a class="add_comment" id="add_comment" href="#">
      <button type="button" class="btn btn-dark float-right" title="Add Comment" style="margin-left:10px; margin-right:10px;" href="#" id="addcoment">
      <i class="fas fa-comment" style="color:white"></i>
      </button>
      </a>
      </div>
      <div class="card-body" id="hideandviewcomments">
      <p class="card-text">
      <ul>{% for entry in item.comments %}
      <li>{{entry.comment}}</li>
      {% endfor %}
      </ul>
      </p>
      </div>
</div>
</div>
</div>
<br>
{% endfor %}