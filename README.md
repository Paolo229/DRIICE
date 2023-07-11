# DRIICE

<html>
<!DOCTYPE html>
<html>
<head>
    
    <title>Connexion et Inscription</title>
    <style>
    body{background-color:  #302536;}
        .hidden {
            display: none;
        }
        button{ background-color: green;
        }
       .conx{background-color: red;
       border: none;
       width: 150%;
       height: 65px;
       font-size: 50px;
       animation: animer 3s;}
       .ins{ width: 150%;
       
       border: none;
       height: 65px;
       font-size: 50px;
       animation: animer 4s;}
        .visible {
            display: block;
        }
        .oub{ background-color: #000080;
        color: white;
        font-size: 50px;
        border: none;
        border-radius: 20px;
        }
        .hy{color:gray}
        .low{color: gray}
        .new{ background-color: #000080;
        color: white;
       font-size: 50px;
       border: none;
      border-radius: 20px;
       }
        ::placeholder { color: gray; 
         font-size: 50px; }
         h1{text-align: center;}
         h2{ text-align: center;
         } 
         img{width: 100%;
         height: 40%;
         margin: 4%;
         margin-right: -10%;
         margin-left: 20%;
         padding:0%;
         animation: animer linear infinite 5s}
         input{border: none;
         border-bottom: solid 1px gray;}
       .mp{font-size: 50px;}
        fieldset{
        padding: apx;
        margin-top: 20%;
        background-color: #302536;
        border: none;
        border-left:solid 5px blue;
        border-radius: 1px;
        border-top: solid 0px green;}
        input { border-radius: 10px;
        width: 150%;
        height: 15%; }
        @keyframes animer{
        0%{filter: opacity(0%)}
        50%{filter: opacity(30%)}
        100%{filter:opacity(60%)}
        }
        footer{color: gray;
        margin-bottom: %;}
        hr{
        border: solid 1px gray;}
    </style>
</head>
<body>

<img src="Hrs.jpg">
<fieldset>
    
    <div>
        <button class="conx" onclick="showLoginForm()">Connexion</button>
        <p><br>
        <button class="ins" onclick="showSignupForm()">Inscription</button>
    </div>

    <form id="loginForm" class="hidden">
      <p></p>
      <hr> 
      <h2 class="hy">Connexion</h2>
      <hr>
        <input type="text" placeholder="Nom d'utilisateur" required>
        <p></p>
        <input type="password" placeholder="Mot de passe">
        <p></p>
        <button class="oub" type="submit"><strong>Se connecter</button></strong>
        <a href="#" ><h1 class="mp">Mot de passe oublié</a></h1>
    </form>

    <form id="signupForm" class="hidden">
    <hr>
    <h2 class="low">Inscription</h2>
    <hr>
       <label> <input type="text" placeholder="Nom d'utilisateur" required></label>
       <p></p>
       <label> <input type="email" placeholder="Adresse e-mail" required></label>
       <p></p>
     <label>   <input type="password" placeholder="Mot de passe"><label>
     <p></p>
        <button class="new" type="submit"><strong>S'inscrire</button></strong>
    </form>
    <br>
</fieldset>


    <script>
        function showLoginForm() {
            document.getElementById("loginForm").classList.remove("hidden");
            document.getElementById("signupForm").classList.add("hidden");
        }

        function showSignupForm() {
            document.getElementById("signupForm").classList.remove("hidden");
            document.getElementById("loginForm").classList.add("hidden");
        }
    </script>
</body>
</html>

