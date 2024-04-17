# Solar-System
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Solar System</title>
    <style>
        body{
            background-image: url("img/Milkeyway.png");
            background-size: cover;
        }
        .comman{
            position: absolute;
            animation-iteration-count: infinite;
            animation-timing-function: linear;
        }
        .sun{
            width: 100px;
            height: 100px;
            background-image: url("./img/sun.png");
            border-radius: 100px;
            margin: 250px auto;
            background-size: cover;
            position: relative;
        }
        .marcury{
            width: 50px;
            height: 50px;
            border-radius: 50px;
            background-image: url("img/Mercury.png");
            background-size: cover;
            bottom: 25px;
            right: -100px;
            animation-name: mercuryanimation;
            animation-duration: 2s;
            transform-origin: -108px center;
        }
        @keyframes mercuryanimation{
            to{
                transform: rotateZ(0deg);
            }
            from{
                transform: rotateZ(-359deg);
            }
        }
        .venus{
            width: 70px;
            height: 70px;
            background-image: url("img/Venus.png");
            border-radius: 70px;
            background-size: cover;
            bottom: 13px;
            right: -220px;
            animation-name: venus;
            animation-duration: 3s;
            transform-origin: -266px center;
        }
        @keyframes venus{
            0%{
                transform: rotateZ(0deg);
            }
            100%{
                transform: rotateZ(359deg);
            }
        }
        .earth{
            width: 80px;
            height: 80px;
            background-image: url("img/Earth.png");
            border-radius: 80px;
            background-size: cover;
            bottom: 10px;
            right: -350px;
            transform-origin: -358px center;
            animation-name: earth;
            animation-duration: 4s;
        }
        @keyframes earth{
                to{
                    transform: rotateZ(0deg);
                }
                from{
                    transform: rotateZ(-359deg);
                }
        }
        .moon{
            width: 25px;
            height: 25px;
            background-color: #7d7373;
            border-radius: 25px;
            background-size: cover;
            bottom: 30px;
            right: -30px;
            animation-name: moon;
            animation-duration: 1s;
            transform-origin: -56px center;
        }
            @keyframes moon{
                0%{
                    transform: rotateZ(0deg);
                }
                100%{
                    transform: rotateZ(359deg);
                }
            }
    </style>
</head>
<body>
    <div class="sun">
        <div class="comman marcury"></div>
        <div class="comman venus"></div>
        <div class="comman earth">
            <div class="comman moon"></div>
        </div>
    </div>
</body>
</html>
