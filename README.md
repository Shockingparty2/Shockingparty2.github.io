<html lang="en">
<head>
<title>CSS Template</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
  background-color: rgba(144, 238, 144, 0.3);
}

/* Style the side navigation */
.sidenav {
  height: 100%;
  width: 200px;
  position: fixed;
  z-index: 1;
  top: 0;
  left: 0;
  background-color: #111;
  overflow-x: hidden;
}


/* Side navigation links */
.sidenav a {
  color: white;
  padding: 16px;
  text-decoration: none;
  display: block;
}

/* Change color on hover */
.sidenav a:hover {
  background-color: #ddd;
  color: black;
}

/* Style the content */
.content {
  margin-left: 200px;
  padding-left: 20px;
}

/* add logo to top of page*/
.logo {
  width: 400px;
  height: auto;
}

</style>
</head>
<body>

<div class="sidenav">
  <a href="https://shockingparty2.github.io">Main Page</a>
  <a href="https://shockingparty2.github.io/page2">ESP task information</a>
  <a href="https://shockingparty2.github.io/page3">ESP task tips</a>> 
</div>

<div class="content">
  <img 
    src="https://assets.nolimits.ukri.org/chelmsford_college_logo_a9a6927a9b.png" 
    alt="Chelmsford College logo"
    class="logo">



<div class="content">

  <img
    src="https://assets.nolimits.ukri.org/chelmsford_college_logo_a9a6927a9b.png"
    alt="Chelmsford College logo"
    class="logo">

  <h2></h2>

  <p>
    <b><mark>WELCOME to this first page of the ESP information general stuffs okay?</mark></b>
    <br><br>
    This website will give you a general idea on the ESP and some tips which helped me to get through the year myself
  </p>

  <!-- CONTACT FORM -->
  <h2>Further Information</h2>

  <form onsubmit="return checkForm()">

    <label>Name:</label><br>
    <input id="name" type="text" required><br><br>

    <label>Email:</label><br>
    <input id="email" type="email" required><br><br>

    <label>Message:</label><br>
    <textarea id="msg" required></textarea><br><br>

    <button type="submit">Submit</button>

    <p id="error"></p>

  </form>

  <!-- JAVASCRIPT -->
  <script>
  function checkForm() {

    let n = document.getElementById("name").value.trim();
    let e = document.getElementById("email").value.trim();
    let m = document.getElementById("msg").value.trim();

    if (!n || !e || !m) {
      document.getElementById("error").textContent =
        "Please fill in all fields.";
      return false;
    }

    document.getElementById("error").innerHTML =
      'This form does not work. However, you can contact the college <a href="https://www.chelmsford.ac.uk/" target="_blank">here</a>.';

    return false;
  }
  </script>

</div>

</body>
</html>
