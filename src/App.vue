<template>
    <div id="app">
        <main>
            <div class="search-box">
                <input type="text" class="search-bar" placeholder="Search Country Here ...">
            </div>
            <div class="weather-wrap">
                <div class="location-box">
                    <div class="location">Dhaka, BD</div>
                    <div class="date">Monday 20 January 2022</div>
                </div>
                <div class="weather-box">
                    <div class="temp">10 C</div>
                    <div class="weather">Rain</div>
                </div>
            </div>
        </main>       
    </div>
</template>

<script>
export default {
    name: "App",
    data(){
        return {
            api_key: `f799225195f29fe1bfe3bf2421c4220d`,

        }
    }
}
</script>

<style>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body{
    font-family: 'Poppins', sans-serif;
}

#app{
    background-image: url('./assets/cold-bg.jpg');
    background-size: cover;
    background-position: bottom;
    transition: 0.4s;
}

main{
    min-height: 100vh;
    padding: 35px;
    background-image: linear-gradient(to bottom, rgba(0,0,0,0.25), rgba(0,0,0,0.75));
}
.search-box{
    width: 100%;
    margin-bottom: 30px;
}
.search-box .search-bar{
    display: block;
    width: 100%;
    padding: 15px;
    color: #080101;
    font-size: 18px;
    appearance: none;
    border: none;
    outline: none;
    background: none;

    box-shadow: 0 0 10px #ff00ea7c;
    background-color: rgba(255, 255, 255, 0.87);
    border-radius: 15px 0 15px 0;
    transition: 0.6s ease-in-out;
}

.search-box .search-bar:focus{
    background-color: #ffff;
    border-radius: 0 15px 0 15px;
    box-shadow: 0 0 18px rgba(248, 54, 190, 0.829);
}
.location-box{
    text-align: center;
}

.location-box .location{
    color: #fff;
    font-size: 32px;
    font-weight: 500;    
    text-shadow: 1px 3px rgba(0, 0, 0, 0.25);
}
.location-box .date{
    color: #fff;
    font-size: 20px;
    font-weight: 300;
    font-style: italic;
}
.weather-box{
    text-align: center;
}
.weather-box .temp{
    display: inline-block;
    padding: 10px 25px;
    color: #fff;
    font-size: 102px;
    font-weight: 900;
    text-shadow: 3px 6px rgba(0, 0, 0, 0.25);
    background-color: rgba(255, 255, 255, 0.25);
    border-radius: 15px;
    margin: 30px 0;
    box-shadow: 3px 6px rgba(0, 0, 0, 0.25);
}
.weather-box .weather{
    color: #fff;
    font-size: 48px;
    font-weight: 700;
    font-style: italic;
    text-shadow: 1px 3px rgba(0, 0, 0, 0.50);
}

</style>
