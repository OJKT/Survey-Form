# Survey-Form
Challenge 2
<style>
  @import url(https://fonts.googleapis.com/css?family=Khand:500);

html,body {
  background-color: #FC5555;
  text-align: center;
  font-family: font-family: "Khand", sans-serif;
  min-width: 400px;
}

h1{
  font-size: 30px;
}

header {
  font-size: 50px;
  font-weight: bold;
  margin: 30px;
}

p {
  font-size: 20px;
}

sub-title {
  font-size: 70px;
  font-weight: bold;
  margin: 30px;
}

h2 {
  font-size: 70px;
  font-weight: bold;
  margin: 30px;
}

#form-outer {
  background-color: rgb(208, 208, 208);
  margin-top: 50px;
  margin-left: 25%;
  margrn-bottom: 50px;
  border-radius: 40px;
  height: auto;
  max-height: 1000px;
  width: 75%;
  max-width: 1000px;
  padding: 10px;
  padding-top: 20px;
  border: 2px solid red;
}

.labels {
  display: inline-block;
  font-family: "Khand", sans-serif;
  text-align: right;
  width: 40%;
  padding: 5px;
  vertical-align: top;
  margin-top: 10px;
}

.rightTab {
  display: inline-block;
  text-align: left;
  width: 48%;
  vertical-align: left;
}

.input-field {
  height: 20px;
  width: 280px;
  padding: 5px;
  margin: 10px;
  border: 1px solid #c0c0c0;
  border-radius: 2px;
}

#userAge {
  width: 40px;
}

.userRatings,
input[type="checkbox"] {
  float: left;
  margin-right: 5px;
}

#submit {
  background-color: #FC5555;
  border-radius: 4px;
  color: white;
  font-size: 1em;
  height: 40px;
  width: 96px;
  margin: 10px;
  border: 2px solid red;
}

.dropdown {
  height: 35px;
  width: 140px;
  padding: 5px;
  margin: 10px;  
  margin-top: 15px;
  border: 1px solid #c0c0c0;
  border-radius: 2px;
}

.radio, .checkbox {
  position: relative;
  left: -43px;
  margin-left: 10px;
  display: block;
  padding-bottom: 10px;
}

footer{
  
}

@media screen and (max-width: 833px) {
  .input-field {
    width: 80%;
  }
  select {
    width: 90%;
  }
}

@media screen and (max-width: 520px) {
  .labels {
    width: 100%;
    text-align: left;
  }
  .rightTab {
    width: 80%;
    float: left;
  }
  .input-field {
    width: 100%;
  }
  select {
    width: 100%;
  }
}
  </style>
<h1 id="title"><u>" Would you Rather "</u></h1>
<hr>
<h2 id="sub-title">' THE GAME '</h2>
<hr>

<div id="form-outer">
<p id="description"><u>
If you FORFEIT you must share the form with someone over the age of 80. This is totally not a form BUT IS.
  </u>
 </p>
  
<form id="survey-form" method="GET" action="https://crossorigin.me/https://freecodecamp.com">  
<div class="rowTab">
  <div class="labels">
    <label id="name-label" for="name">* Name: </label>
  </div>
  <div class="rightTab">
   <input autofocus type="text" name="name" id="name" class="input-field" placeholder="Enter your name" required>
  </div>
</div>
    
<div class="rowTab">
  <div class="labels">
    <label id="email-label" for="email">* Email: </label>
  </div>
  <div class="rightTab">
    <div class="labels">
      <input type="email" name="email" id="email" class="input-field" required placeholder="Enter your Email">
    </div>
  </div>
</div>
    
<div class="rowTab">
 <div class="labels">
  <label id="number-label" for="number">* Number: </label>
 </div>
  <div class="rightTab">
   <input type="number" name="Contact Number" id="number" min="11" max="12" class="input-field" placeholder="Contact Number">
  </div>
</div>
    
<div class="rowTab">
  <div class="labels">
   <label for="currentPos">Would You Rather Eat...</label>
  </div>
      <div class="rightTab">
        <select id="dropdown" name="currentPos" class="dropdown">
      <option disabled value>Select an option</option>
      <option  value="Upsidedown">Upsidedown</option>
      <option value="MoonDirt">Moon Dirt</option>
      <option value="CatsFur">Cats Fur</option>
      <option value="Maggotsinpie">Maggots in pie</option>
      <option value="Forfeit">Forfeit</option>
        </select>
      </div>
</div>
    
<div class="rowTab">
 <div class="labels">
  <label for="userRating">* Would you complete your chosen ' would you rather eat ' if your money doubled?</label>
 </div>
 <div class="rightTab">
  <ul style="list-style: none;">
   <li class="radio"><label>Definitely<input name="radio-buttons" value="1"  type="radio" class="userRatings" ></label></li>
   <li class="radio"><label>Maybe<input name="radio-buttons" value="2"  type="radio" class="userRatings" ></label></li>
   <li class="radio"><label>Not sure<input name="radio-buttons" value="3"  type="radio" class="userRatings" ></label></li>
  </ul>
 </div>
</div>
    
<div class="rowTab">
  <div class="labels">
    <label for="most-like">Which Superhero/Villan would you most like to be?</label>
  </div>
    <div class="rightTab">
     <select id="most-like" name="mostLike" class="dropdown">
      <option disabled selected value>Select an option</option>
      <option value="Batman">Batman</option>
      <option value="Ironman">Ironman</option>
      <option value="VictorVonDoom">Victor Von Doom</option>
      <option value="DeadShot">Dead Shot</option>
     </select>
    </div>
</div>
    
<div class="rowTab">
 <div class="labels">
  <label for="preferences">Pick Your worst combination<br>(Check only Three): </label>
 </div>
 <div class="rightTab">
  <ul id="preferences" style="list-style: none;">
   <li class="checkbox"><label><input name="prefer" value="1" type="checkbox" class="userRatings">Spiders</label></li>
   <li class="checkbox"><label><input name="prefer" value="2" type="checkbox" class="userRatings">Dark</label></li>
   <li class="checkbox"><label><input name="prefer" value="3" type="checkbox" class="userRatings">Cliff Edge</label></li>
   <li class="checkbox"><label><input name="prefer" value="4" type="checkbox" class="userRatings">Stuck in the middle of the sea</label></li>
   <li class="checkbox"><label><input name="prefer" value="5" type="checkbox" class="userRatings">Rats</label></li>
   <li class="checkbox"><label><input name="prefer" value="6" type="checkbox" class="userRatings">Lots of Dead Babies</label></li>
   <li class="checkbox"><label><input name="prefer" value="7" type="checkbox" class="userRatings">Loud Screaming</label></li>
   <li class="checkbox"><label><input name="prefer" value="8" type="checkbox" class="userRatings">Force Feeding</label></li>
   <li class="checkbox"><label><input name="prefer" value="9" type="checkbox" class="userRatings">Diseased Enviroment</label></li>
   <li class="checkbox"><label><input name="prefer" value="10" type="checkbox" class="userRatings">Only Person Alive</label></li>
   <li class="checkbox"><label><input name="prefer" value="10" type="checkbox" class="userRatings">Blood, lots of BLOOD</label></li>
  </ul>
 </div>
</div>
    
<div class="rowTab">
 <div class="labels">
  <label for="comments">Any Comments or Suggestions for " would you rather's "</label>
 </div>
  <div class="rightTab">
   <textarea id="comments" class="input-field" style="height:50px;resize:vertical;" name="comment" placeholder="Enter your comment here..."></textarea>
  </div>
</div>

<div class="rowTab">   
  <button id="submit" type="submit">Submit</button>
</div>
<footer>&copy; 2018 OJKT Styles</footer>
</form>
