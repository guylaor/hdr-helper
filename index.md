<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-uWxY/CJNBR+1zjPWmfnSnVxwRheevXITnMqoEIeG1LJrdI0GlVs/9cVSyPYXdcSF" crossorigin="anonymous">

    <title>HDR helper</title>
  </head>
  <body>
 
<main>

  <div class="px-4 py-5 my-5 ">
    <h1 class="display-5 fw-bold text-center">HDR Helper Page</h1>

    <div class="container">
  <!-- Stack the columns on mobile by making one full-width and the other half-width -->
  <div class="row">
    <div class="col-md-8">
    
    <video id="videoplayer" style="width:100%;" controls   >
        
    </video>
    
<div class="mb-3">
  <label for="formFile" class="form-label">Select Video File (H.264 / H.265)</label>
  <input class="form-control" type="file"  id="videoinputfile">
</div>

    </div>
    
    
    <div class="col-6 col-md-4 text-left">
    <!-- right cell -->
       <ul class="list-group list-group-flush ">
        <li class="list-group-item text-left">An item</li>
        <li class="list-group-item">A second item</li>
        <li class="list-group-item">A third item</li>
        <li class="list-group-item">A fourth item</li>
        <li class="list-group-item">And a fifth one</li>
        </ul>
    </div>
  </div>




    <!--
    <div class="col-lg-6 mx-auto">
      <p class="lead mb-4">Quickly design and customize responsive mobile-first sites with Bootstrap, the world’s most popular front-end open source toolkit, featuring Sass variables and mixins, responsive grid system, extensive prebuilt components, and powerful JavaScript plugins.</p>
      <div class="d-grid gap-2 d-sm-flex justify-content-sm-center">
        <button type="button" class="btn btn-primary btn-lg px-4 gap-3">Primary button</button>
        <button type="button" class="btn btn-outline-secondary btn-lg px-4">Secondary</button>
      </div>
    </div>
    -->
  </div>

<script>

const fileInput = document.getElementById('videoinputfile');
const player = document.getElementById('videoplayer');
fileInput.onchange = () => {
  const selectedFile = fileInput.files[0];
  console.log(URL.createObjectURL(selectedFile));
  player.src = URL.createObjectURL(selectedFile);
}

</script>


    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-kQtW33rZJAHjgefvhyyzcGF3C5TFyBQBA13V1RKPf4uH+bwyzQxZ6CmMZHmNBEfJ" crossorigin="anonymous"></script>
  </body>
</html>