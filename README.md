# JCjenson-in-spaaaace # Redefine the html_content since it was lost between cells

html_content = """

<!DOCTYPE html>

<html lang="en">

<head>

  <meta charset="UTF-8">

  <title>Callbackping Glitch</title>

  <style>

    body {

      background: #111;

      color: #ccc;

      font-family: monospace;

      display: flex;

      flex-direction: column;

      align-items: center;

      justify-content: center;

      height: 100vh;

      transition: all 0.5s ease-in-out;

    }



    input {

      padding: 1em;

      font-size: 1.5em;

      border: 2px solid #555;

      background: #000;

      color: #0f0;

      margin-bottom: 20px;

    }



    .glitch-text {

      font-size: 2em;

      text-shadow: 2px 2px red, -2px -2px blue;

      animation: flicker 0.2s infinite;

      white-space: pre-wrap;

    }



    .final-msg {

      color: white;

      font-size: 3em;

      text-align: center;

      margin-top: 30vh;

      animation: pulse 1s infinite;

    }



    @keyframes flicker {

      0% { opacity: 1; }

      50% { opacity: 0.1; }

      100% { opacity: 1; }

    }



    @keyframes pulse {

      0%, 100% { transform: scale(1); }

      50% { transform: scale(1.05); }

    }



    .glitch {

      background: black !important;

      color: red;

    }

  </style>

</head>

<body>

  <input id="callbackInput" placeholder="ping a universe..." />

  <div id="glitchBox"></div>



  <script>

    document.getElementById('callbackInput').addEventListener('keypress', function (e) {

      if (e.key === 'Enter') {

        const input = this.value.toLowerCase();

        if (input.includes('murder drones') || input.includes('minecraft') || input.includes('doors')) {

          startGlitchSequence(input);

        }

      }

    });



    function startGlitchSequence(input) {

      document.body.classList.add('glitch');

      const glitchBox = document.getElementById('glitchBox');



      let glitchText = '';



      if (input.includes('murder drones')) {

        glitchText = "v̴̖̫̳̺̻̺̱͕́͠ė̵̖̖͌͘̚̚n̵̖͕̮̙̹̐̀̀̑̐͊̔̈́͠͠g̸̠̀̿̑̾͝ē̷̢̡̱̞̹̬̳͙̳̬̎̐̿̍a̶͔̻̲͙̩̝̍́͗̓̒͊̓̈́̈́̕͘͠n̸̩̯̳͕͉̬̟͛͆͛͘͝c̷̡̺̰̼̪͓̠̱͈̩̞̱̜͒͌͑͐͝ẽ̶͓͖̘̥͇͓̺̳̺̬̜̤̓͛̌̎̎͂͝...";

      } else if (input.includes('minecraft')) {

        glitchText = "c̸̛͕̯͂̐̓͗͊͛͝ȟ̸̨̯̲̝̳͓͎̭͖͊̄̔̽̓̂̋̇̋̀̕̚͜i̵͚̩̞̐̈͘e̷̘͕̪̳̾̽̆̅̏̾͌͘̚͘͠͝f̷̢̬͉̘̰͙̫̙̥̘͇̈́̇̔̾̊̈́̽̍͑̈́̆͐̅͋͝. I am Steve. W̵̛̜̠͛͌͐̒̋̈́̐̈́́̃͠e̴̛̟̬̲̍̓̈́̾͌͌̽̕͝͝͝l̴̛̺͉̞̤̙͚̇͂͌̇̅̎̍̚c̸̢̡̛̛͓͖̯̲͚̩͎̞̬̠̯̏͗̅̄͑̌̾́̿̕͘͜o̸̢̤̗̗̿̓͛̆̈́͘m̴̡̛̦͕̞̤͈̝͉͎̺̮̹͔̈́̈́̑̈́͆͝e̸̛͚͉̬̹̩̝͚̅͆̎̏̈́̐̋̑̐͘͘͝͝";

      } else if (input.includes('doors')) {

        glitchText = "T̸̢̟͎͓͍͉͈̺̟̼̮̼̟̬͓̰̯̹̝̹̞̮̈́͌̿͒̾͋̽̋͛͋̈́̓̒̓͂̓͆͆̽͆̀͐̇͘͘͜͝h̴̢̡͉̩̬͙̳͚̯͈̘̳̝̖̯̮͚̍̌̑̽́̊͛̅̀̐̒̀͒̐̋̒͌͘̕̕̚e̵̤̗̝͖̰͕͕̗̰̪̳͙͉̥̱͍̫̘͎̰̖͇͚̥̦̩͎̓̐̓̑̿̅̍̍͗͋͗̒̐͗͘͘̕͝ ̸̛̞͇̘͔͙͕͕̮̙̰̭̼̺̞̰̟̝̘̝̳̤̼͕̹̈́̀̾͊̾͐͐͛̾̋̒̒̽̽͒̍́̾́̓́̽̚̕͜͜͝͝h̸̡̡̡̢̛̻̖̫̦̠̮͈̗̹͇̞͖͎͔̤̜̥̱̲̤̞̻̜̺̻̲̖̗̱͍̮̯̥̤̱̖̟̻̗̞̘̝̑̓̄̑̑̈́͑̅͆̈́̍̾͑͂̀̿̽͆͌̅̀̚͘͝͝͝͠͝ơ̶̢̢̢̡̛̛̜̮̰͙̦̥̰̲͓̤͖͖̹̲̠̥͓͉̲̮͔̯̥͎̱̦̞̱͓̯̟̑͋̍́̓̽͆̓͒͛̈͌̐͆̿̏̎̓͗̈́̀͋̐͗͛̔̈́̔̍̇͂͊̅͘͘͜͝͠͝r̶̡̢̡̢̢̛̛̛̗͙̘̤̗̼̹͚͙̗̥̝̠̤̤̹̼̰̙̬͓̜͓̦̤̗͓̟̺͉̫̝̞̖̼̮̹͇̤̰̥̼̗̩͕̰̞̲̲̹͉͌͗̎̈́̓̓͛́͌͗̊͐͒̓̏͗̌̓͐̔̈́́̈́̓͘͘̕͜͜͠͝r̵̡̡̢̮̖͎̠͉͉̖͕͇͚̺̪̗̟̩̙͉͖̹̱͉̖̳̘̟͉͓͙̞̥̠̟̘̖̖̟͇͔͉̝͇̓͋̐̋̋͌̾͗͋̾͐̿̐͗͒̓̏̍̿́́͗̀̓̾̎̾̍͗͘̚̕͜͠͝͝ͅơ̴̢̢̡̢̢̢̤̬̯͓̞͈͕͇͕͚͙̬̦̰͖̰̜̤̦̳͙̫͇̪͈̼͉͇͇̖̟̜̟͎̲̠̤̇̑̄̌͆̔̾̐͛̄̓͒͌̎̌̑͌́̄̽͂͗̒͒̌̑̒̔͆̈́͌͊̉͋̍͊͐̚͘͘̕̚̚͜͜͜͜͜͝͝͠ͅr̴̡̢̨̨̛͎̝͔̙̞̬̪̗͎͙̼̜̟̤͉̜̫̮͓̺͚͕̘͉̙̘͚̰̬̪̻̟͎͎̙̠̗̬̜̟̲̳̰͙̗̦̗͉͍̘̮̙̩̞̼̭̈̄̽̇͂͛̎̍̌̍̾͊̎̌̎̏̿̑́̄̇̒͂̉̌̑͂̌̎́̾͊̌͐̄̋͂̈́̈́̾͛̈́̚͘̕̕͘̕͜͜͜͜͠͝͝ͅs̷̡̛̺̩͖̳̬̼̘̫̦̙̞͓̳͇̠͕̖͍͍͓͚̖͔͖͕̹̲̖͇͉̼̬̩͉̳͈͖̤̼͚͓͈͚̮͈͎̜̋͌̋̀̓̌͐͗̍̌͐̍͋̓̄͂̅͐͒́̈́̄͗̊̀́̍̄̋̈́̌͗̓̊͋̇͗͋̿́̚͘̚̚̕͜͜͜͝͝͝͝ ̶̨̢̛̛̹̲͖̩̝͙̪̠̪̯͇̝̤̟̼̠͓͚̝̱̩͇̜͓̫̘͚̫͉̺̳̞͔̳͈̳̬̖̤̥̰͓̯͐̈́̄̾̽̓͌̒̅̇̊͌̍̑̐̄͆̏̓̊̓̏̉͋̒̅̍̄̓̎̿́̑̒̔̐̅̇̿̿̿̈́̏̒͌͗̈́̅̕͘̚̕͝͠͝͝͝͠ͅa̷̢̛̜͔͚̖̩͖͉̙̟͍͓̠̜̼̝͍̳͈͖̳̙͓̝̩͔̼͕̠̞̺̹̙̲̮̺̠͚̙̰͕͙̩̪̗͕̮͈̗̹̰̹̗̞̤͎̟̤̝͖͚̗̞̠̲̰̖̘̭̗̼̬̍͗́͆̈́̀͒͐̆͗̾̓͋̈́̈́̄̓̾̽̒̌́͋̉̔̓͒͒̋̉̽̐͒̾̆͗͌̉̎̄͗̀̑̌͋̒͋̏̈́͒́̇͗͂͛̐̅͊͋̑͂̕̕͘̚͘͜͝͠͝͝͠͝͝r̷̢̛̖͍͉̳͎̲̘͙̫̹̰͔̯͖͍͍͓͕̘̞̯̜̮̦̩̩͇̱̟̝͕̯̪̩͔͇͇̖̟̹̼̠͇̳̙̻̼̼̤̪̯̮̹̝͇̈́̓̋͛̓̈́͂̿̑͗̓́́̐̈́͂͐͛̈́̈́́̿̈́̒́̿͂̄̓̓̐̐̆̈́̏̐͛͒̆̇̀͒͋̐̇̈́̿͆̄̈́͐͒́̌̇͑̏̒̇͂̽̇̔͛̽̌̋̒͌̑̅̚̚̚̚͘͘̚̚͜͝͠͠͝e̷̢̛̛̞͈͙̗̼͉̬͎̙̩̦̬̼̘͓͚͓͈̤͓͕̹̥͎̦͉̮̖̫̮̟̖̰̗̠͔̼͈̬͔͎̘̗̙̗̘̤̞̠̗̬̮̳͔͎͚̠̗͙͍͗͐̀̏̓̏̆̓͌͛̀̓̿̓̇͐̄̎̈́̀̓̈́͆̓͂̉́̈́̍̏̈́̿͑̒̆̒̾̄̓̑̈́̅̍̓̐̈́͋͗̿̄̇̓̌̾̅̏̓̐̐̌̔̒̓̎͆̍̚̕̕̕̕͘̚͜͝͝͝ͅͅ";

      }



      glitchBox.className = 'glitch-text';

      glitchBox.textContent = glitchText;



      setTimeout(() => {

        glitchBox.innerHTML = "<div class='final-msg'>YOU SHOULD NOT HAVE DONE THAT</div>";

      }, 3000);

    }

  </script>

</body>

</html>

"""



# Save to file

file_path = Path("/mnt/data/callbackping_glitch.html")

file_path
