# Modern-Type-Login-Form
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form Design</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            width: 100vw;
            height: 100vh;
            display: flex;
            background: url(https://images.unsplash.com/photo-1575936123452-b67c3203c357?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxzZWFyY2h8Mnx8aW1hZ2V8ZW58MHx8MHx8fDA%3D)no-repeat;
            background-position: center;
            background-size: cover;
            align-items: center;

            justify-content: center;
        }

        .wrapper {

            width: 400px;
            height: 500px;
            background: rgba(0, 0, 0, 0.5);
            border-radius: 40px;
            border: 3px solid rgba(0, 0, 0, 0.2);
            box-shadow:0 0  20px #fff;

            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;

        }

        h2 {
            color: #fff;
            text-transform: uppercase;
            padding: 20px 0;
            font-size: 2em;
        }

        .form-group {
            position: relative;
            /* background-color: red; */
            border-bottom: 3px solid #fff;
            width: 330px;
            margin: 30px 0;
        }

        .form-group input {

            width: 100%;
            height: 50px;
            background: transparent;
            border: none;
            outline: none;
            color: #fff;
            font-size: 1.2em;
            padding: 0 30px 0 10px;
        }

        input:focus ~ label,
        input:valid ~ label {
            top: -5px;
        }

        .form-group label {

            position: absolute;
            top: 50%;
            left: 10px;
            transform: translateY(-50%);
            font-size: 1.2em;
            color: white;
            transition: 0.5s;
        }

        .form-group span {
            position: absolute;
            top: 50%;
            right: 10px;
            transform: translateY(-50%);
            color: #fff;
        }

        p {
            text-align: center;
            color: white;
            padding: 10px 0;



        }

        p>a {
            color: white;
            text-decoration: none;
            font-weight: 600;
        }

    p>a:hover{
        text-decoration: underline;
        font-style: italic;
        color: blue;
    }

    #btn{
        width: 100%;
        height: 50px;
        border-radius: 40px;
        border: none;

        text-transform: uppercase;
        font-size: 18px;
        font-weight: 600;

    }

    #btn:hover {
        background-color: blue;
        color: white;

    }
    </style>
</head>

<body>

    <div class="wrapper">

        <h2>Login</h2>
        <form action="">
            <div class="form-group">
                <input type="email" required>
                <label for="">Email</label>
                <span><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="icon"
                        viewBox="0 0 16 16">
                        <path
                            d="M.05 3.555A2 2 0 0 1 2 2h12a2 2 0 0 1 1.95 1.555L8 8.414zM0 4.697v7.104l5.803-3.558zM6.761 8.83l-6.57 4.027A2 2 0 0 0 2 14h12a2 2 0 0 0 1.808-1.144l-6.57-4.027L8 9.586zm3.436-.586L16 11.801V4.697z" />
                    </svg></span>
            </div>
            <div class="form-group">
                <input type="password" required>
                <label for="">Password</label>
                <span><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                        class="bi bi-lock-fill" viewBox="0 0 16 16">
                        <path fill-rule="evenodd"
                            d="M8 0a4 4 0 0 1 4 4v2.05a2.5 2.5 0 0 1 2 2.45v5a2.5 2.5 0 0 1-2.5 2.5h-7A2.5 2.5 0 0 1 2 13.5v-5a2.5 2.5 0 0 1 2-2.45V4a4 4 0 0 1 4-4m0 1a3 3 0 0 0-3 3v2h6V4a3 3 0 0 0-3-3" />
                    </svg></span>
            </div>

            <p><input type="checkbox"> Remember Me
                <a href="#">Forget Password</a>
            </p>

            <input id="btn" type="button" value="Login">
            <p>Don't have an account? <a href="#">Ragister</a></p>


        </form>

    </div>

</body>

</html>
