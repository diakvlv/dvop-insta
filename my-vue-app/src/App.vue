<script setup lang="ts">
interface Data {
  elements: { title: string, image: string }[]
}

import LinkWeather from './components/linkWeather.vue';
import RightHead from './components/rightHead.vue';
import PreviewTemp from './components/previewTemp.vue';
import MiddleInf from './components/middleInf.vue';

const data: Data = {
  elements: [
   { title: 'Logo', image: '../public/cuacane-logo.png' },
    { title: 'Dashboard', image: '../public/dashboard-logo.png' },
    { title: 'Map', image: '../public/map.png' },
    { title: 'Saved Location', image: '../public/saved-location.png' },
    { title: 'Settings', image: '../public/settings.png' },
    { title: 'Logout', image: '../public/logout.png' },
    { title: 'Calendar', image: '../public/calendar.png' },
    { title: 'Rain Chance', image: '../public/rain-chance.png' },
    { title: 'UV index', image: '../public/UVIndex.png' },
    { title: 'Wind', image: '../public/wind.png' },
    { title: 'Pressure', image: '../public/pressure.png' }
  ]
}
</script>


<template>
  <!--<div>
        <a href="https://vitejs.dev/" target="_blank">
                <img src="/vite.svg" class="logo" alt="Vite logo" />
              </a>
              <a href="https://vuejs.org/" target="_blank">
                <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
              </a>
            </div>-->
  <div class="wrapper">
    <div class="leftContainer">
      <div class="left-column">
        <div class="left-column">
  <div class="logo">
    <ul class="logo-ul">
      <li><br></li>
      <li><br></li>
      <li><img src="cuacane-logo.png" alt="Cuacane"></li>
    </ul>
  </div>
  <ul class="menu">
    <li><a href="#" class="active"><img src="dashboard-logo.png" alt="Dashboard">Dashboard</a></li>
    <li><a href="#"><img src="map.png" alt="Map">Map</a></li>
    <li><a href="#"><img src="saved-location.png" alt="Saved Locations">Saved Locations</a></li>
    <li><a href="#"><img src="calendar.png" alt="Calendar">Calendar</a></li>
    <li><a href="#"><img src="settings.png" alt="Settings">Settings</a></li>
  </ul>
  <div class="logout">
    <img src="logout.png" alt="Log Out">
    <a href="#">Log Out</a>
  </div>
</div>
</div>

    </div>
    <div class="middleContainer">

            <div class="search">
         <div class="searchBar">
          Willkomen
         </div>
         <div class="lupa">
          <a href=""><img src="https://cdn-icons-png.flaticon.com/512/1167/1167092.png" alt=""></a> 
        </div>
        <div class="lupa">
          <a href=""><img src="https://cdn-icons-png.flaticon.com/512/40/40031.png" alt=""></a>  
        </div>
      </div>
      <div class="middle1">
        <div class="lev">
         <div class="blank">
          <div class="text-left">
            Gotham
          </div>
          <div class="text-left1">
            1016hPa
            </div>
          </div>
          <div class="blank">
          <div class="tempBig">
            14°
          </div>
          <div class="text-middle">
           Polojasno
            </div>
        </div>
          <div class="blank">
          <div class="text-right">
            Monday
          </div>
          <div class="text-right2">
           20kph
            </div>
          </div>
        </div>
     
        <div class="obr">
          <img
            src="../src/assets/temp.PNG">
        </div>
      </div>


      
      <div class="window-section">
  <div class="window">
    <div class="text-container">
      <div class="row1"><b>Wind</b></div>
      <div class="row2">Today wind speed</div>
      <div class="row3"><b>12km/h</b></div>
    </div>
    <img src="wind.png" alt="Image 1" class="image">
  </div>
  <div class="window">
    <div class="text-container">
      <div class="row1"><b>Rain Chance</b></div>
      <div class="row2">Today rain chanse</div>
      <div class="row3"><b>24%</b></div>
    </div>
    <img src="rain-chance.png" alt="Image 2" class="image">
  </div>
  <div class="window">
    <div class="text-container">
      <div class="row1"><b>Pressure</b></div>
      <div class="row2">Today Pressure</div>
      <div class="row3"><b>720 hpa</b></div>
    </div>
    <img src="pressure.png" alt="Image 3" class="image">
  </div>
  <div class="window">
    <div class="text-container">
      <div class="row1"><b>UV Index</b></div>
      <div class="row2">Today UV Index</div>
      <div class="row3"><b>2</b></div>
    </div>
    <img src="UVIndex.png" alt="Image 4" class="image">
  </div>
</div>

    </div>
    <div class="rightContainer">
        <div class="right">
      <RightHead head1="<" head2="Head" head3=">" />
        <br><br><br>
      <div class="prev">
        <PreviewTemp temparature="17" city="Prag"
          image1="https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/Eo_circle_light-blue_blank.svg/2048px-Eo_circle_light-blue_blank.svg.png"
          image2="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Yellow_icon.svg/2048px-Yellow_icon.svg.png" />
        <PreviewTemp temparature="14" city="Prag"
          image1="https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/Eo_circle_light-blue_blank.svg/2048px-Eo_circle_light-blue_blank.svg.png"
          image2="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Yellow_icon.svg/2048px-Yellow_icon.svg.png" />
        <PreviewTemp temparature="13" city="Prag"
          image1="https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/Eo_circle_light-blue_blank.svg/2048px-Eo_circle_light-blue_blank.svg.png"
          image2="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Yellow_icon.svg/2048px-Yellow_icon.svg.png" />
        <PreviewTemp temparature="13" city="Prag"
          image1="https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/Eo_circle_light-blue_blank.svg/2048px-Eo_circle_light-blue_blank.svg.png"
          image2="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Yellow_icon.svg/2048px-Yellow_icon.svg.png" />
      </div>
<br><br><br>
      <LinkWeather name="Praha" temparature="21"
        image1="https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/Eo_circle_light-blue_blank.svg/2048px-Eo_circle_light-blue_blank.svg.png"
        image2="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Yellow_icon.svg/2048px-Yellow_icon.svg.png" />
      <LinkWeather name="Brno" temparature="13"
        image1="https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/Eo_circle_light-blue_blank.svg/2048px-Eo_circle_light-blue_blank.svg.png"
        image2="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Yellow_icon.svg/2048px-Yellow_icon.svg.png" />
      <LinkWeather name="Ostrava" temparature="18"
        image1="https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/Eo_circle_light-blue_blank.svg/2048px-Eo_circle_light-blue_blank.svg.png"
        image2="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Yellow_icon.svg/2048px-Yellow_icon.svg.png" />
      <LinkWeather name="Olomouc" temparature="21"
        image1="https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/Eo_circle_light-blue_blank.svg/2048px-Eo_circle_light-blue_blank.svg.png"
        image2="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Yellow_icon.svg/2048px-Yellow_icon.svg.png" />
      <LinkWeather name="Liberec" temparature="14"
        image1="https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/Eo_circle_light-blue_blank.svg/2048px-Eo_circle_light-blue_blank.svg.png"
        image2="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Yellow_icon.svg/2048px-Yellow_icon.svg.png" />
      <LinkWeather name="Karlovy Vary" temparature="21"
        image1="https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/Eo_circle_light-blue_blank.svg/2048px-Eo_circle_light-blue_blank.svg.png"
        image2="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Yellow_icon.svg/2048px-Yellow_icon.svg.png" />
      <LinkWeather name="J. Hradec" temparature="13"
        image1="https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/Eo_circle_light-blue_blank.svg/2048px-Eo_circle_light-blue_blank.svg.png"
        image2="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Yellow_icon.svg/2048px-Yellow_icon.svg.png" />
      <LinkWeather name="Jihlava" temparature="12"
        image1="https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/Eo_circle_light-blue_blank.svg/2048px-Eo_circle_light-blue_blank.svg.png"
        image2="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Yellow_icon.svg/2048px-Yellow_icon.svg.png" />
      <LinkWeather name="Chomutov" temparature="21"
        image1="https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/Eo_circle_light-blue_blank.svg/2048px-Eo_circle_light-blue_blank.svg.png"
        image2="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Yellow_icon.svg/2048px-Yellow_icon.svg.png" />
      </div>
    </div>
  </div>
</template>
<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300&display=swap');


* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: 'Roboto', sans-serif;
  }
  
.prev {
  display: flex;
    gap: 20px;
    justify-content: space-between;
    padding: 0 20px;
}

.middleContainer {
  width: 60%;
  background-color: white;
  border-right: 1px solid #ecf3f8;
}

.wrapper {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.rightContainer {
  background-color: white;
  width: 25%;
}

.leftContainer {
  width: 15%;
  background-color: white;
  border-right: 1px solid #ecf3f8;
}

.left-column {
  height: 100vh;
  background-color: white;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
}

.logo-ul {
  list-style: none;
  font-size: 25px;
  margin: 0;
  display: flex;
  align-items: center;
}

.logo img {
  width: 165px;
  height: 50px;
  margin: 20px 0;
  display: inline; 
}

.menu {
  list-style: none;
  padding: 20px 0;
  margin: 0;
}

.menu li {
  margin-bottom: 10px;
}

.menu a {
  display: flex;
  align-items: center;
  color: #333;
  text-decoration: none;
  padding: 10px;
  transition: background-color 0.3s ease;
}


.menu a.active {
  font-weight: bold;
}

.menu img {
  width: 20px;
  height: 20px;
  margin-right: 10px;
}

.logout {
  display: flex;
  align-items: center;
  margin-bottom: 20px;
}

.logout img {
  width: 20px;
  height: 20px;
  margin-right: 10px;
}

.logout a {
  color: #333;
  text-decoration: none;
}



.window-section {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
  height: 400px;
  background-color: white;
  padding: 20px;
}

.window {
  width: 45%;
  height: 45%;
  background-color: #ecf3f8;
  border-radius: 15px;
  margin-bottom: 20px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

.text-container {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: flex-start;
  padding: 20px;
}

.row1 {
  font-size: 20px;
}

.row2 {
  font-size: 16px;
}

.row3 {
  font-size: 20px;
}

.image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}




.right{
  background-color: white;
}

.middle1 img{
  border-radius: 20px;
}
.lupa{
  margin: 15px;
}
.blank{
  background-color:  #303c54;
}
.searchBar{
 align-items: center;
  margin: 10px;
  background-color: white;
  height: 30px;
  padding-top: 0.5%;
  border-radius: 20px;
  padding-left: 40px;
  width: 80%;
}
.search{
 height: 60px;
  margin: 40px;
  padding-top: 10px;
  border-radius: 25px;
  display: flex;
}
.text-middle{
  background-color: #303c54;
  text-align: center;
  padding-left: 10px;
}
.tempBig {
  background-color: #303c54;
  padding-top: 40%;
  width: 120px;
  text-align: center;
  font-size: 80px;
  padding-left: 10px;
}
.lupa img{
  width: 30px;
}
.lev {
  background-color: #303c54;
  width: 50%;
  padding: 20px;
  flex-direction: row;
  display: flex;
}

.text-left {
  background-color: #303c54;
  margin-left: auto;
}
.text-right2{
  padding-top: 280px;
  background-color: #303c54;
  text-align: center;
  margin-left: auto;
}
.text-left1{
  background-color: #303c54;
  padding-top: 280px;
  text-align: center;
  margin-left: auto;
}
.text-right {
  background-color: #303c54;
 margin-left: auto;
}

.middle1 {
  display: flex;
  padding: 50px;
  margin: 40px;
  height: 340px;
  background-color: #303c54;
  border-radius: 20px;
  color:white;
  min-height: 450px;
  min-width: 500px;
}

.obr {
  height: 350px;
  border-radius: 40px;
}

.obr img {
  object-fit: cover;
  width: 100%;
  height: 100%;
}

.prev {
  display: flex;
  gap: 20px;
  justify-content: space-between;
  padding: 0 20px;
  background-color: white;
}

.mod {
  flex-direction: column;
}

.RightHead {
  height: 100px;
}

</style>