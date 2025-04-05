# week-4-Asignment-
Web Development week 4 assignment .Grid and flexbox Layout 

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox and Grid Layout</title>

    <style>

        *{
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        body{
            font-family: Arial, sans-serif;
            line-height: 1.6;
            color: #333;
        }
        header{
            background-color: #333;
            color: white;
            padding: 1rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        nav ul {
            list-style: none;
            display: flex;
            gap: 1rem;
    }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
    }
        .container{
            display: grid;
            grid-template-columns: 1fr 3fr;
            gap: 2rem;
            padding: 2rem;
        }

        .sidebar{
            background-color: #f4f4f4;
            padding: 1rem;

        }
        .main-content{
            background-color: #e9ecef;
            padding: 1rem;

        }
        footer{
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1rem;
            margin-top: 2rem;
        }
        /* Media Queries */
    @media (max-width: 768px) {
      .container {
        grid-template-columns: 1fr;
      }

      nav ul {
        flex-direction: column;
        gap: 0.5rem;
      }
    }

    @media (max-width: 480px) {
      header {
        flex-direction: column;
        align-items: flex-start;
      }
    }
      nav ul {
        align-self: flex-start;
      }
    </style>
</head>
<body>
    <header>
        <h1>Mutton Den Limited</h1>
    
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About Us</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Contact Us</a></li>
        </ul>
    </nav>

</header>

<div class="container">
    <aside class="sidebar">
        <h2>Choma Zone</h2>
        <p>One of the best delicacy in the company that most of us I believe love to enjoy eating with our family and friends </p>
    </aside>

    <main class="main-content">
        <h2>Fried Beef and Mutton</h2>
        <p>This being one of the best meal for most of our staffs members I believe that all our clients will love everything the meal.</p>
    </main>
</div>


    <footer>
        <p>Designed by Lisa</p>
    </footer>

</body>
</html>
