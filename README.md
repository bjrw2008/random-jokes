<!DOCTYPE html>
<html lang="en">


<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Joke Generator</title>
    <link rel="stylesheet" href="styles.css">
    <style type="text/css">
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;300;400;500&display=swap');

*{
     box-sizing: border-box
}

body {
    background-color: #1f1d2b;
    font-family: 'Poppins', Arial, sans-serif;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    margin: 0;
}
.container {
    background-color: #ffd791;
    border-radius: 10px;
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1), 0 6px 6px rgba(0,0, 0, 0, 0.1);
    padding: 50px 20px;
    max-width: 100%;
    width: 800px;
    text-align: center;
}
h3 {
  margin: 0;
  letter-spacing: 2px;
  opacity: 0.5;

}
.joke {
    font-size: 30px;
    line-height: 40px;
    margin: 50px auto;
    max-width: 600px;
}

.btn {
  background-color: #660033;
  border: 0;
  border-radius: 10px;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1), 0 6px 6px rgba(0,0, 0, 0, 0.1);
  color: #fff;
  cursor: pointer;
  font-size: 16px;
  padding: 14px 40px;
}

.btn:active{
  transform: scale(0.98);
}

.btn:focus {
  outline: 0;
}
    </style>
</head>
<body>

    <div class="container">
        <h3>Random Jokes Generator</h3>
        <div id="joke" class="joke">
            Here's the joke for you
        </div>
        <button id="get_joke" class="btn">
            Get another joke
        </button>
    </div>
    <script src="script.js"></script>
    <script>const jokeEl = document.getElementById('joke')
const get_joke = document.getElementById('get_joke');

get_joke.addEventListener('click', generateJoke);
generateJoke();

async function generateJoke(){
    
    });

    const joke = await jokeRes.json();

    jokeEl.innerHTML = joke.joke;
}</script>

</body>
</html>
