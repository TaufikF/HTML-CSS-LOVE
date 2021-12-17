# HTML-CSS-LOVE

```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Document</title>
    <style>
        * {
            margin: 0px;
            padding: 0px;
            box-sizing: border-box;
            max-width: 100% !important;
        }

        h1 {
            position: absolute;
            font-size: 100px;
            color: #fff;
        }

        body {
            font-family: sans-serif;
            background-color: #fff;
            overflow: hidden;
        }

        .wrap-love {
            position: relative;
            width: 150px;
            height: 150px;
            margin: 25% auto 0 auto;
            animation: love 2s infinite alternate;
        }
        
        .love {
            position: absolute;
            width: 100%;
            height: 100%;
            background-color: #e47e7e;
            -webkit-transform: rotate(-45deg);
            -ms-transform: rotate(-45deg);
            transform: rotate(-45deg);
        }

        .love::before,
        .love::after {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            border-radius: 50%;
            background-color: #e47e7e;
        }

        .love::before {
            top: -50%;
            left: 0;
        }

        .love::after {
            top: 0;
            left: 50%;
        }

        @keyframes love {
            0% {
                transform: scale(1);
            }

            50% {
                transform: scale(2);
            }

            100% {
                transform: scale(3);
            }
        }

        p {
            text-align: center;
            margin-top: 10%;
            animation: p 2s infinite alternate;
            color: #fff;
        }

        @keyframes p {
            
            0% {
                transform: scale(1);
            }

            50% {
                transform: scale(2);
                color: #e47e7e;
            }

            100% {
                transform: scale(3);
                color: #fff;
                text-shadow: 0 0 5px #e47e7e, 0 0 10px #e47e7e;
            }
        }

        h1 {
            margin-top: -10px;
            font-size: 50px;
            text-align: center;
            animation: h1 2s infinite alternate;
        }

        @keyframes h1 {
            
            0% {
                color: #e47e7e;
            }

            50% {
                color: #a15656;
            }

            100% {
                color: #fff;
            }
        }
    </style>
</head>
<body>
    <div class="wrap-love">
        
        <div class="love"></div>
        <h1>For You!!!</h1>
    </div>    
    
    <p>@By - M Taufik Fadillah</p>
</body>
</html>
```
