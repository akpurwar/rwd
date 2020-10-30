<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        html,body{
            width:100%;
            height: 100%;
            margin:0;
        }

        .nav{
            border-bottom: 1px solid blanchedalmond;
            text-align: right;
            height: 70px;
            line-height: 70px;
        }

        .menu{
            margin: 0 30px 0 0;
        }

        .menu a{
            text-decoration: none;
            color: gray;
            margin:0 10px;
            line-height: 70px;
        }
      
      label{
          margin: 0 40px 0 0 ;
          font-size: 26px;
          line-height: 70px;
          display: none;
      }

      #toggle{
          display:none;
      }

      @media only screen and ( max-width:500px ){
          label{
              display:block;
              cursor:pointer;
          }
          .menu{
              text-align: center;
              width:100%;
              display:none;
          }

          .menu a{
              display: block;
              border-bottom: 1px solid wheat;
              margin :0;
          }

          #toggle:checked + .menu{
              display:block;
          }
      }

    </style>
</head>
<body>
    <div class="nav">
        <label for="toggle">&#9776;</label>
        <input type="checkbox" id="toggle">
    </input>
    <div class="menu">
        <a href ="#">Home</a>
        <a href ="#">About Us</a>
        <a href= "#">Contact</a>

    </div>
    </div>
</body>
</html>
