# cyclistic_casestudy
Capstone Project (Google Data Analytics Course): Cyclistic Ridership Case Study 

## Documentation

[File 1](#file-1) | [File 2](#file-2) | [File 3](#file-3)

---

### File 1
Detailed documentation for File 1 goes here.

---

### File 2
Detailed documentation for File 2 goes here.

---

### File 3
Detailed documentation for File 3 goes here.


<div class="tab">
  <button class="tablinks" onclick="openTab(event, 'file1')">File 1</button>
  <button class="tablinks" onclick="openTab(event, 'file2')">File 2</button>
  <button class="tablinks" onclick="openTab(event, 'file3')">File 3</button>
</div>

<div id="file1" class="tabcontent">
  <h3>File 1 Documentation</h3>
  <p>This is the documentation for File 1.</p>
</div>

<div id="file2" class="tabcontent" style="display:none">
  <h3>File 2 Documentation</h3>
  <p>This is the documentation for File 2.</p>
</div>

<div id="file3" class="tabcontent" style="display:none">
  <h3>File 3 Documentation</h3>
  <p>This is the documentation for File 3.</p>
</div>

<script>
function openTab(evt, fileName) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(fileName).style.display = "block";
  evt.currentTarget.className += " active";
}
</script>
