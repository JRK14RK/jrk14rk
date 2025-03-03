<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Page</title>
    <!-- Font Awesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* -----------------------------------------------
        login page Style
        Name  : Misbahul Fahmi Fahrezi
        Youtube : Go For Edu
        Date    : 30 Oktober 2020
        Updated : [Current Date]
        ----------------------------------------------- */

        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            overflow-y: hidden; /* Hide vertical scrollbar */
            overflow-x: hidden; /* Hide horizontal scrollbar */
        }

        .login-container {
            background-color: #fff;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            width: 300px;
            text-align: center;
        }

        .logo {
            margin-bottom: 30px;
        }

        .logo img {
            max-width: 100%;
            height: auto;
        }

        .input-group {
            position: relative;
            margin-bottom: 20px;
        }

        .input-group input {
            width: 100%;
            padding: 10px 15px 10px 40px;
            border: 2px solid #ccc;
            border-radius: 25px;
            box-sizing: border-box;
            transition: border-color 0.3s;
        }

        .input-group input:focus {
            border-color: #E9762B;
            outline: none;
        }

        .input-group i {
            position: absolute;
            top: 50%;
            left: 15px;
            transform: translateY(-50%);
            color: #888;
        }

        .tombol {
            width: 100%;
            padding: 10px;
            background-color: #E9762B;
            border: none;
            border-radius: 25px;
            color: #fff;
            font-size: 16px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .tombol:hover {
            background-color: #d96423;
        }

        #timer {
            color: #D91656;
            margin-bottom: 20px;
            font-size: 14px;
        }

        @media (max-width: 400px) {
            .login-container {
                width: 90%;
            }
        }
    </style>
</head>
<body>
    <div class="login-container">
        <div class="logo">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTSut2lbnrdOuIz0xhqubWhsDGffd5WO3sVHA&s" alt="Logo">
        </div>
        <form name="myform" method="post">
            <div class="input-group">
                <i class="fas fa-user"></i>
                <input type="text" name="uname" class="inputtext" autocomplete="off" placeholder="Username" required>
            </div>
            <div class="input-group">
                <i class="fas fa-lock"></i>
                <input type="password" name="pass" class="inputtext" autocomplete="off" placeholder="Password" required>
            </div>
            <div id="timer"></div>
            <input type="button" class="tombol" name="log" id="logbutton" value="Log in" onclick="myfunction()">
        </form>
    </div>

    <script type="text/javascript">
        function myfunction() {
            var un = document.forms["myform"]["uname"].value;
            var pw = document.forms["myform"]["pass"].value;
            if (un === "admin" && pw === "adminjrk14rk") {
                // Redirect to the specified URL in the same tab
                window.location.href = 'https://sites.google.com/view/resorjembatan14rangkasbitung/menu-laporan';
            } else if (un=="FAJRIN" && pw=="54686") {
// Redirect to the specified URL in the same tab
    window.location.href =('https://sites.google.com/view/resorjembatan14rangkasbitung/fajrin');
}

else if (un=="RISWAN" && pw=="71079") {
                // Redirect to the specified URL in the same tab
    window.location.href =('https://sites.google.com/view/resorjembatan14rangkasbitung/riswan');
}

else if (un=="DIDI" && pw=="52620") {
                // Redirect to the specified URL in the same tab
    window.location.href =('https://sites.google.com/view/resorjembatan14rangkasbitung/didi-umyadi');
}
else if (un=="AGUS" && pw=="72022") {
                // Redirect to the specified URL in the same tab
    window.location.href =('https://sites.google.com/view/resorjembatan14rangkasbitung/agus');
}
else if (un=="ARIF" && pw=="71121") {
                // Redirect to the specified URL in the same tab
    window.location.href =('https://sites.google.com/view/resorjembatan14rangkasbitung/arif');
}
else if (un=="ARI" && pw=="KAPM") {
                // Redirect to the specified URL in the same tab
    window.location.href =('https://sites.google.com/view/resorjembatan14rangkasbitung/ari');
}
else if (un=="HOIR" && pw=="KAPM") {
                // Redirect to the specified URL in the same tab
    window.location.href =('https://sites.google.com/view/resorjembatan14rangkasbitung/hoir');
}
else if (un=="LOHYASIN" && pw=="KAPM") {
                // Redirect to the specified URL in the same tab
    window.location.href =('https://sites.google.com/view/resorjembatan14rangkasbitung/lohyasin');
}
else if (un=="DEDI" && pw=="KAPM") {
                // Redirect to the specified URL in the same tab
    window.location.href =('https://sites.google.com/view/resorjembatan14rangkasbitung/dedi');
}
else if (un=="TARIPIN" && pw=="55407") {
                // Redirect to the specified URL in the same tab
    window.location.href =('https://sites.google.com/view/resorjembatan14rangkasbitung/taripin');
}
else {
                document.getElementById("timer").innerHTML = "Salah password";
                setTimeout(function() {
                    document.getElementById("timer").innerHTML = "";
                }, 3000); // Clear error message after 3 seconds
            }
        }
    </script>
</body>
</html>
