---
title: Notebook Remaining Calculation
tags: nb, notebook
categories: Javascript
---


# Notebook Remaining Calculation

<p><input id="buy" style="width: 120px;" type="date" /> <input id="resign" style="width: 120px;" type="date" /> <input id="subsidy" style="width: 120px;" type="text" placeholder="請輸入金額" /> <button id="clickBtn" class="button">計算</button></p>
<div>
<p style="display: inline;">購買日期為:</p>
<p id="1" style="display: inline;"> </p>
<br />
<p style="display: inline;">離職日期為:</p>
<p id="2" style="display: inline;"> </p>
<br />
<p style="display: inline;">使用天數為:</p>
<p id="3" style="display: inline;"> </p>
<br />
<p style="display: inline;">應付天數為:</p>
<p id="4" style="display: inline;"> </p>
<br />
<p style="display: inline;">二年天數為:</p>
<p id="5" style="display: inline;"> </p>
<br />
<p style="display: inline;">應付金額為:</p>
<p id="6" style="display: inline;"> </p>
<p style="display: inline;"> </p>
<p style="display: inline;"> </p>
</div>
<script>// <![CDATA[
var click = document.getElementById("clickBtn");

function display(){
    var buy = document.getElementById("buy").value;
    var resign = document.getElementById("resign").value;
    var buyCul = new Date(buy);
    var resignCul = new Date(resign);
    var duringUsed = Math.abs(resignCul - buyCul) / (1000 * 3600 * 24);
    var duringDay = 730 - duringUsed;
    var subsidy = document.getElementById("subsidy").value;
    document.getElementById("1").innerHTML = buy;
    document.getElementById("2").innerHTML = resign;
    document.getElementById("3").innerHTML = duringUsed;
    document.getElementById("4").innerHTML = duringDay;
    document.getElementById("5").innerHTML = 730;
    document.getElementById("6").innerHTML = parseInt((duringDay / 730) * subsidy);
}

click.addEventListener("click", display);
// ]]></script>