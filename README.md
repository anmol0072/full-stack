<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Registration Form</title>

    <style>
        body {
            font-family: Arial;
            background: #f2f2f2;
        }

        form {
            height: 300px;
            width: 400px;
            margin: 50px auto;
            padding: 25px;
            background: white;
            border-radius: 6px;
            box-shadow: 0 0 8px rgba(0,0,0,0.1);
        }

        h2 {
            text-align: center;
        }

        input {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            border: 2px solid #ccc;
            border-radius: 50px;
            box-sizing: border-box;
        }

        input:invalid {
            border-color: red;
        }

        p {
            color: red;
            font-size: 14px;
            display: none;
            margin: 5px 0 10px;
        }

        input:invalid:focus + p {
            display: block;
        }

        button {
            padding: 10px 20px;
            background: red;
            color: white;
            border: none;
            border-radius: 5px;
            float: none;
            cursor: pointer;
        }
    </style>
</head>

<body>

    <form>
        <h2>Student Registration</h2>

        <label>Full Name:</label>
        <input type="text" required minlength="9" maxlength="50" pattern="[A-Za-z ]">
        <p>Must contain 9–50 letters</p>

        <label>Email:</label>
        <input type="email" required>
        <p>Valid email required</p>

        <label>Age:</label>
        <input type="number" required min="16" max="30">
        <p>Age 16–30 only</p>
        <hr>

        <button type="submit">Register</button>
    </form>

</body>
</html>
