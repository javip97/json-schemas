<div id="tabs">
  <button class="tablinks" onclick="openTab(event, 'Tab1')">Tab 1</button>
  <button class="tablinks" onclick="openTab(event, 'Tab2')">Tab 2</button>
  <button class="tablinks" onclick="openTab(event, 'Tab3')">Tab 3</button>
</div>

<div id="Tab1" class="tabcontent">
  <h3>Tab 1 Content</h3>
  <p>This is the content of Tab 1.</p>
</div>

<div id="Tab2" class="tabcontent">
  <h3>Tab 2 Content</h3>
  <p>This is the content of Tab 2.</p>
</div>

<div id="Tab3" class="tabcontent">
  <h3>Tab 3 Content</h3>
  <p>This is the content of Tab 3.</p>
</div>

<script>
function openTab(evt, tabName) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(tabName).style.display = "block";
  evt.currentTarget.className += " active";
}
</script>
