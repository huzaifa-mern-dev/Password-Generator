# Password-Generator
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Password Generator by Huzaifa</title>
    <style>.inputBox {
  position: relative;
}

.inputBox i {
  position: absolute;
  top: 16px;
  right: 6px;
  color: #000;
  font-size: 28px;
  cursor: pointer;
  z-index: 2;
}

.passBox {
  background: #fff;
  border: none;
  padding: 10px;
  width: 300px;
  border-radius: 5px;
  font-size: 20px;
  margin-block: 8px;
  text-overflow: ellipsis;
  font-weight: 400;
}

.row {
  margin-block: 8px;
  display: flex;
}

.row p,
.row label {
  flex-basis: 100%;
  font-size: 18px;
}

.row input[type="checkbox"] {
  width: 20px;
  height: 20px;
}

.genBtn {
  border: none;
  background-color: #000;
  padding: 12px 24px;
  color: #fff;
  font-size: 18px;
  margin-block: 8px;
  font-weight: 700;
  cursor: pointer;
  border-radius: 5px;
  transition: all ease 500ms;
}

.genBtn:hover {
  background-color: #5b1010;
  color: #000;
}
</style>
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"
    />
  </head>
  <body>
    <div class="container">
      <h1>Password Generator</h1>
      <div class="inputBox">
        <input type="text" class="passBox" id="passBox" disabled />
        <i class="fa-solid fa-copy" id="copyIcon"></i>
      </div>
      <input type="range" min="1" max="30" value="8" id="inputSlider" />
      <div class="row">
        <p>Password Length</p>
        <span id="sliderValue"></span>
      </div>

      <div class="row">
        <label for="lowercase">Include lowercase Letter (a-z)</label>
        <input type="checkbox" name="lowercase" id="lowercase" checked />
      </div>
      <div class="row">
        <label for="uppercase">Include uppercase Letter (A-Z)</label>
        <input type="checkbox" name="uppercase" id="uppercase" checked />
      </div>
      <div class="row">
        <label for="numbers">Include numbers (0-9)</label>
        <input type="checkbox" name="numbers" id="numbers" checked />
      </div>
      <div class="row">
        <label for="symbols">Include symbols Letter (!@#)</label>
        <input type="checkbox" name="symbols" id="symbols" checked />
      </div>
      <button type="button" class="genBtn" id="genBtn">
        Generator Password
      </button>
    </div>
    <script src="scipt.js"></script>
  </body>
</html>
